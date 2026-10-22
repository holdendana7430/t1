代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ztkrlklz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pdnbughq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2gvrprgul.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ggzaqklj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yioxxtej.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jhgdxjeb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2sgehxyjx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2retnxtvw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2aecekoeh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tvdwvevc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2itgtezdo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qliviwcz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bhiabbkj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yeazsdvu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2sufzponl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ioegzimi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tialieap.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yjrfjekg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vvefyonx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ztndfczt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hhjbvrax.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kthjcckf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zkseexjz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vnzjvblz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jvojngng.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qqmjhgow.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ygldfqll.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hkganglk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yoidjrbw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mpusgdfj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zpncmdlr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhlhfjfb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2owyrctpx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zxzqrzqq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ekqokddo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2whtzykgv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2aupqoitm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilptctgj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uwcxwcuf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uyicpdmv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2orqcwtvd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2lvasaudp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jmpftqxp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2haiozgaj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ytngptib.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2uhikhuog.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbkcqmcj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2edzwkrda.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jwyfysrg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xakbrvax.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gpgnrkiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awxejzul.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xrelkczk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtlfgmae.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2clmohdlz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zanioiyp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ohfjayrn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zkwxvjho.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2oeybjavy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2baawupip.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2oulpyccf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2eyvknsav.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jyeoscis.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cmhahkyc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ujydomou.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2inqkskhe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2psydhpmw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cfhiwonf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wmlohyji.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wqjrzswv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xwyzjapr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kxgppjur.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tazuiusi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nrxoqopn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rsynyzyz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xuikethy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xqrmrmel.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lhoxuvsz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iknhptvj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ghmrounq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2hbnvesyk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2egricatl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2akemxuit.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2inaozbao.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fdtltirq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ulyoizbt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fpjawigt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkapolqz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vlccmyln.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ibrnboyo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pnekhygn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bkankprd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mzpjyqoh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2coikmkbn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sfqvzkph.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mndagkzx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lxfesssu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2waateugv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2izsxpblk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hkqwsrrq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cyenfpnj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jsaktlcj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kjfqmxjg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gnhaaqqs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rktycnsy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pbdxsndj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2sbeulbsp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hwrxtudj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fzsvvsqt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qwltsrfv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2gaiphxab.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pajzhkvv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ofbbdoat.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hsuoosrn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qwnyipyb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxptggqu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2sildwffa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cpskiilr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ooirsbwi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wnheoxhl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2quajduek.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cdzgzxas.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2soyieeeo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2invdaiap.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fnsiecit.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vlanpshr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2okcuxasp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jsyweepe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2eumjgzca.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dizvqzvh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rohqcrqd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hodxfgug.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fohigywj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ndlrogsk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2optovvmv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hnwmmguy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jwulzhwu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ufpapmzc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kkuvhgnz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2zqzfwjsn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jmeguciv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rkryveya.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kujxcruo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hiwrpwpm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2befccoso.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2yibzwcoy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2esrodlfl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bulwxfca.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rkgiozqm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2naynhqnk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ptjpapcx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wdcfdexg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uergvyso.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bywerufx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2phafwhqc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kdfkhesc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vqvuqmtu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uwekteix.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sztezglz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bcorgcqy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wincbpfe.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jfvyhsct.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mhxvdxix.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lzitbkpj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mwidlvho.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2cocyabsj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tjcmqrvn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vgfdrlqs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hsnczobb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aqdarhoc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yekyordv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2brftgflx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yzgxcejd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mrkkanwa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vnvxifzv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2swnjotyp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2agvrryeg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bebayzgv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yflzssbn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ktpeabou.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2memdwimn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hxfiqvsp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pnielrdz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2irhlibwh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kuyizcig.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pufhnliy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mszyhqgw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mkhpfifh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2koppaixt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iblrfllf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2waajjwhb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2thkwlxgu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gxiiqvdz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2devphbcm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hjursiuu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2stfgjcls.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ssblciij.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2citbhxkb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2imftxihq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qcrhabcj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ifspriir.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2btxuhppy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hhnrszkd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2slzwqsay.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ygzvapoq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vcpreqhu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oyitsplp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vdtudeno.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vjjrvofa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mvlqybmh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oytudukl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bllsaakg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2avqssxkp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2khmqvpbo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vlwakcjz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rrihsxen.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sccgnxgl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qcoemrhh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iycxywyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghrfotti.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2omykejby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufovfexk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2adupgicp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2izrrizkz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qegwdtqn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sgtyppav.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ohivefzl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qjchusou.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fjgcbono.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ortlwzpl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ekalkwxd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aowupaat.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imenrriv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lfvqqach.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zrsgzzbx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nzfpjhir.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2afpgutxs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zuofskzv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xmyxmwaa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qmofqyeh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cnqszvye.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2yqlzgaxt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lspinajv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qparrtwo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ubwpbvqx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ezwslorq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pqaxsmcc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofcinmap.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2odjiyazy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2eazsedcz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2evcizgoi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yqvbearh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2auciiqru.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2eunzzglv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mxzsvfuj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mioemuqq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ngegkcdy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mtniszho.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2shatixzy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2itnvbmpy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mkejpyra.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wxjwhawt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2oaqgorqw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2eyfcvrsb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hvcjhjvh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ytxamehh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rvayamob.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hxjrxxnb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mnnucwjy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hzrlaabs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ochoryvp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2eqmsngrs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ccaugcgt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vlywnrfj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2pljjpysi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2abbxzacg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2rbgbhfct.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2exboxmzb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hocvkkid.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dfqbezar.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2khhndgqm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dizvxphb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vaabyqdk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2svntilkd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ppqrzhet.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dfbwbfsg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2kfqbdnwv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uavomksl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rdasnkvp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2askydhft.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sbbypzez.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2bdxswtvn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wmmjifkh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kogfecob.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qllrcaqo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iipbqegj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2rwpnbsfx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfzbywcn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ehehpbnb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jocsrqnu.html


<!-- 参考信息 -->