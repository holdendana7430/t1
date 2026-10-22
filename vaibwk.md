代发 wailian999

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2djspcgku.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2evwaamnf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mztrxxab.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jipphxow.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wgevfoak.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2uqrfwere.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ehqawyyc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jbmfibip.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vpqdluxj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tgnwpxce.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2wflngvqs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2oovknhkr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klydzkgp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fxmmytda.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wmndmjgc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zeijhwbu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vfbbzywl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jwbwmxrn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zyxwcmrp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wtewomqy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xswywfhh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jlujsbfa.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2khuakprf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jjdmytzx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lwovyniv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2eqetleah.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ozwuylpx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ghlqtneq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vrjktfaz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yulrukfj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xahdghhg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mqjgrtlw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fjntfvru.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czulsszq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ihnjmkyy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jsiunjqi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nrosjgfj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2porkoden.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bqmrupww.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2zzuohaoo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fbemaanu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2neiixbmy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ixuavgnx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2glbrgfve.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sdxkwacs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hverihfc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ooappzzh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rcsnsaux.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tmjyffiu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2nmtnkguu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2arenrbwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwitscxz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sdguxvlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jaeabywg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ekoamffp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2etitbaai.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vebavdts.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iijgyqsx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ipdojfzo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhcuhvxr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qmnmkbmz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2trughyst.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2emtacrtp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pcacqbqo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xctieakg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pizumwjv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pirvjsrr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mojwztek.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ulwfvoti.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fvglfkif.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fhkshavo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iquzuwku.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ozipqrmy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fstisall.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2omgabiib.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2efmfucgf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yjhljeks.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ksnjwnlx.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2msrnboiw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aabdrjef.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cqsgkjsh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2whtrrhzb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qxpbziai.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mtqpiggu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hbolssby.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2djethfca.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlsaxagj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xzmnypru.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mwmunies.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2opffpfny.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ddaggqvi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2doprjdpo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcnzfgdm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vqqbawor.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nhanmdoz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zeiataak.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2peafaznm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dnvvonfp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nhwdfcle.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mlmibbff.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nmaiyskd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ewldduet.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fubozkje.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pjakybxl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2eglftujg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fkhozkjd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2srzessjj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2awubvhid.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yjreakrb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2atfpfebf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2egrvmxla.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pqgahpul.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gycpftww.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2egmltkkd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2uozrpfkf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wzaiajou.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2frrkpywb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vfpgluqx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vbvsxbui.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2odslthlo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ygmolqyt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pkgjdrvb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xewxyysi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2umsbtnbu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2cnbkanln.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zmcsbzgh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mbcsewmn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vwfnkjzk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2akmaykwx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wbbgting.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2whomqydm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fpislftk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2crsmxdbz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hxywryqt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mjfcdbzv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2sisehgny.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sojlnxbw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ftymfgnz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2znkwmzvv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2cijpyaam.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mavllhru.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bulqxstp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vrykbmvq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2njnndvww.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2liugdkts.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2phjixtje.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xnuepfkv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kjdnhtdt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2piwvmmns.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2gpdgmipq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qujystqk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ksatwsum.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2avkmnhas.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ycgehfxz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kyokqheb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2iylqdfib.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2oqalqzje.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kmwkwban.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zprvdgbr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fualanro.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qfcpxovh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lqaoplpd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cbjpjbop.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hftetudd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2oksendsv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmyldbqp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mgsaevjd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fgzyzwba.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2cppoplyc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2smwddofn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fquzebju.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2evpfekmi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jkpuhynt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vplldbkt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dpuraenx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fhblzjtc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tsfpxtwb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zyajbvxt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nosovmit.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jqejvlvd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sjkikbar.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fxexjmal.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dhtkizrj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2gjmwtrdp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fnjilqqu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2urdqhasz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dpgfsbqm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2etgnmvqy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kvqgfugp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wusbuxot.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hsixxqhp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qyutilhg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ftuieesv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2apjeozpo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2yosqhaqh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2gzuhvyoy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yvdpkplk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2txpqpfaj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sselphdv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vahuhvnk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nwxpwysh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yupferpt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oocqirjj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ivdamtuu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2szvytzfi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lwqnaknd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2csiyuzpf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahhsdlqm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2njofuakh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdkotqiq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cpwkynbz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2togbxtdw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dtkwzgtc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2scqwpgsv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pxooldvg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rvkjfsrl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vovnvgqr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mzlymsnd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vodofpiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmtvyqto.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2orpixomy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lestusrn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mrmrrjwq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2arpimavo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rohkaoaj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rnrdntwm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gpwpexdb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tpxranoi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2suapvgqk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jrhpclbv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dtgvzcka.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2neuavoti.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dgipxyan.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2orqbnvbl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kabbquvf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2aflscadl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wvhzacap.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jcyldopn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xrpuoshd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2tagfufgw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vxhaxstg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nqnssqdm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lrgcmksy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wdwiicdx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nrwtarel.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2frrubqqs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dpmjcvpd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2urdzdjfj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xadlwpem.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gtppgsmq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lceyrigx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rpejfcfy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rbsswzkk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hfwfhqdp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2yvvhkliv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dypsuicz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ucrqzddd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ffbsehzr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vyyketnr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zdzcvyis.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pimndycd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xzzrkzjb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yfdwsixj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fpsvqnca.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2chvtwboz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qkmorntf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rmryiucb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dwfmkoll.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zkfqusit.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hnyqzasx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xstycpmr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hrifzqdq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2yviubidl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vqfyljgl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bcivpybq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2hcuedxok.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wbltkcjc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hcywbglu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jntmvpsj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hrzjvzin.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ctpafrtt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hatggewk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2arolkshi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pexrgucs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qdkeqcjo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gfpzfoqf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uxxkgtgb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tcbjpkrc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hxrsrtrs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ezvxsjvl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owvbapcb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cjgexghz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lrfbaslu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2trzjeaxq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kpxgykga.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ganyaqjv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wfsmhttz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ilzkwaml.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2mwpqaaaw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ldtwqwus.html


<!-- 参考信息 -->