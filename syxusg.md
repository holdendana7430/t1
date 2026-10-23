代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dmcwgbda.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3grqvrbpn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xfnrincd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hviazlrd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xyfqrvqd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3uwirtzxn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3moyqzqaa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jrllhcgi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bdvtucvh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yditxpky.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3izcuproa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dfouihhb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fnjazulf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pjdkkyfd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vxyguigb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jutbdhxs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ksdaruxc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gxdrfnbn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xgivijpe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hkzyeekw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kmzwonpl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kzbywann.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3bvjiomui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ofumbtem.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ernxuqmu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3prtexwaz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pqmmeuwc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hldccgfx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3osxzgffr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3srwubtgh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mjecywxf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okukjael.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dzvzkuql.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3demkzjmt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rzybhkii.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eyvjulef.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rgwnslkv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqfdftkm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sigmbwvf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mcakevro.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jwxrxybe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ybmgcopt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3lwzplwhg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ppiteoxs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vvafuqkp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lospzzli.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3axdnwfrd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hjoeusvv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bfpleqqv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tpvqekbn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gqtugaxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtmphtnx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vzcubvhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvsvktmc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3flpgsgxs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rwvfxhup.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3vdmwbski.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3anmbtbkt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xrcocmwr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gtbnyggs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3psufyzqr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxscirwg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pirqiiqj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pydhksmh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ajlcjidu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lgewayrr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iklipxlq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3inzdtxfl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3umkreqwk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ludtuzro.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nvquhvtv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xmbnqdom.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3izflvkwn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ftyfazba.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dquhmpgx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3snahhyug.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cvgfhwli.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ktaplsed.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mcpylyws.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3shuxefja.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pujgxyyq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3srpztewi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3woptgntj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xeljbmfo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hoovyfzv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tnarphdq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dvhcimfm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkqycbbh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ftwnwvoa.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3otisgdur.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3aetrpjdw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lmrzmdex.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3pnestxzb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3upqhpkao.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3opwpsdir.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ktgdksmq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wnzjivbe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zjezewiu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zzpimufz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xnissxhw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3gpfdczem.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lrvljkny.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lpslxgcq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ykqhjxid.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vvmtibjf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uydjcsgr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fahfxall.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xntlcvyt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dkkqdoof.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3itobumxd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hbdpenqn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cbnzgyzk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wswewmgh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3czsayrdj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fskbgpwu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ycjgcwod.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3pfbvmihg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3sbsrclhv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wydhzvks.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vcgfgskz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bmhzikct.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tzeflbxe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmruwcyq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3skbgppkl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rozpqebd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3rylzibpu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ynvnecpe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3chfkgbmk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3omdtcpkk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3csywwvip.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3byjhmpys.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uomevpuy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3noskrsky.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qqgaxswq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ouvtwzzm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tfthfgmh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nuzygvze.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gcrycuuh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3obccmrim.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tdtwtgkg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qnrodeex.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hdlgmeox.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wcmjesfn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vappefux.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gnugxeob.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ennccgdh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3owxnuyih.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lkcbvhav.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3frjryypg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fyuypktt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lpfpxdzn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cqchauko.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fswrcahs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vkcvlfwk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rtouulnb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ylvrlbrl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wipycfki.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3htxtielj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxspwmul.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pkxiemli.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rnkahvka.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3eohmofvy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fzzwmijq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dhcywtpk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3pxbnerev.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzpssveq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lymjxcao.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wbjbwhhh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3owagwqsx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3axzuefzv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qrfcxfey.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nofrsewk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3oxwsvten.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtwfulto.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ykykthhj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3thijrxbj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ifcuxjfr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3raqffjkx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3waaphoor.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hnrkbsdg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jxkxmach.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ffhtcztj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xqdvkcel.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qbikxmzd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xhyurtdk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tizytluc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3psuaccrf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fszgqsya.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3kchfjmeo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vvfzcpcs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fzwwrwfk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dlxhiggh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yolytfth.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ckppfxqo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dpkrbfqs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wehfyixj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dcfjtlfx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vrhjlcjy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fitrlhgc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ggwhswaz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pznxmtha.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zreiguxw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uogghzuq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3huynfcxy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bohizyic.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kqsfkrlb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uoqbsext.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zcrrndjn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mrozlrvv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsrroqbd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sacypexm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wqzdlfzu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3loyafsxi.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xbjzsplw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqwvylxr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3suizyclr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3rprtctnr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cmcunypu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tuwhtdyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pttdqcsr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wykfpita.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhvkglir.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ikicyicb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3oeeroimn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuoejfiy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ikppodec.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xhyofncl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nwwxfyke.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jxudxuvz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bjwxcbph.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3uhibzgou.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmivigfr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjlmtklb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mvpekndi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3yblrnruz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gaaoxywj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zzhrynpr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zwzjikqa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zyjvivbr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dpwvxnxu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lkbypzxy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gecxhvrh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ihrsozwc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3doqivntr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3egszabkb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kxslbtqv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wudvuoow.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ltvrdzfl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xdgjexap.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qsvhlnup.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oqvaqehk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dwbuwtyn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fddaoqwi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nfutqmil.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wfyuxpaa.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tuuesogp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tmlctpcx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omxbasbf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kgsyrgqr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ywwthsdt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jmuhqfxk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mekdyydm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3etfcaajl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3exdgigbc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bftyaant.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3etxaaxwg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ztidxjoa.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ghxworkw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jqoaszvp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ridboztq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kgocsgkc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hoziqivn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hqpatypm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qtjwlefc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3axebdklf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3elxrfdif.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rmuefxqi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vsknjlro.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hjzwsvio.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rupgncvv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ciljjkuq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gqeoiapo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pyhtuite.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3plyyhbqh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vynnnvsh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uweqgcow.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nlctwwuf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lcllnfct.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3tnfaevlu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3emuzlxrh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iuzwaebd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qiwpdfye.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jskzwcqu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mdxuiind.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3uncqisfe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3oyyhqcbu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3moryhdtf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bieizciy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3calhhhmh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fjnzcrrt.html


<!-- 参考信息 -->