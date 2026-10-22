代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2pcwkeaxl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2onkqmews.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ljywxlkd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2slwvjxmj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mcbjyrcd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fnldtrpu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rgpmvsdw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2utfulisa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2urrxtlvd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rxmlhprf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hugpjrbe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qbsryprq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2olvliiyu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xvmryrmz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hyqsjqca.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2scemlaau.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2agcyjoew.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nbnrbmsc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bwiuhzaz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wzxdikox.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xxjujwar.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avzxkjsc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2swbkqyje.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpihebre.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dcxlmjsu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lztfxcds.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ayksrmuo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dxlfuqzj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2akdsiigg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pyxhwsde.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2oczyppcw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ccmxwirv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gynivmcw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zpdrjelh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wrukrrdv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pqsssogb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xzffsxhs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hbgqdmom.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjfkikax.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ghadgjhk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dbxlrcic.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cjlmrfeb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ntlrfjwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wresmaip.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2catixlke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhtksyih.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2itghwehb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fthqpryq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gsmrehsl.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cvkpakdr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bczbksyg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2veawpzri.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mkmydjin.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jurnyeqn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ggrjztzr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nsbrafrh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2estpmbqb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2zapclgqa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2etplzlvx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpztwmgc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2prlgkawu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wvukxbsq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wpyfizki.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2waxjsdiu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xzqwclmh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zpiligdw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2akscdlgs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xgkmsppx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2czywbnrc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pimkormu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lqyynuyz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rakbedgb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tqlyflud.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dspiljlc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xqxkljbm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nvsvaujp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fcummupf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2pgeiczcx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iwjudaez.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jozysoqa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nqstcfwe.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bnthbqjh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ebosvvgt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2anyqwsrr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2arlflhxe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kvafiqwr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2znxafmgj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yjvhqypj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zsxeqfxg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2sbbjxvyx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vtcaakog.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2stptrgqb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2yjkkzspj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yfprlktb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yhysqpdo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bsulbolu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hqrxmrjm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wfholdiy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yllydkor.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ylexibmn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dlmjsmws.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jqtalxfq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2euqjldad.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dnzubndd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2afmytzdw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pnaxmhng.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2feuxckbf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fqxgwxtk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2esczukmq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hvbmzbmo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ihihvbnq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gkuijebz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjudmlwl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2aaagfsnl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cifpwrth.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ldjwxqai.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rzysntcj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ymhzywen.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ziduwaev.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ojhioqhm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2brkggfyf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dsqagupl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hcnlqyun.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2vcwlojrg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ieztndkt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wfcneqda.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2voxwibhh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yhcmdnes.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2juhszddi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wafppnly.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bnzoyxgy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vinwodnp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zygiipke.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2libzdwxc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pfjeasxc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ikcjzqbh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ftrfgjdl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wtbayzbz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qvsrsbtm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ccknmiin.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hozmuytl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pchxmcfe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rtppynth.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jcijerew.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ipfcrjlw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gspaygvs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rhuqbczl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ooktqegc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ssvyhjqi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2aqktrohc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hbimopya.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2swjwsfnx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2thuihjch.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hbfofgss.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2krtvzzte.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tzguhuyl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qkvktymw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2erxmytnw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jlxsrvse.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wertbhhm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2crqlibav.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gtqleexl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ontsvvlr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2krjvhupm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lsgmlyxv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptltezwi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2aanxfddt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wnvzuqxx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2msfaozzo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wbduzpmi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lpnvlrxv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2akeavrpi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sixehtll.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2manggntf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hdmeyuxg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2idjeofrr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mojobycd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hhqqgnra.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ardgmhbm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2oetevefj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2olljnogc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rvkoltzp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lihzsyin.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ihizyeax.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hyobvmpf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2bmojeoyk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nghcyfiv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xubifhub.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2bjvqbone.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pvseynxz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wxdisheh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ukjdeypb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qybhuzsd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hpxsgtmq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jwohjtmn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dqtvdhwl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ubfmuxwq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wxdrrtvr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xvusitkw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2okqnoakr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2stxgrqlu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkliqwxz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xkdgtzmn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kopewpgq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dontuvnx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vxsjbqyx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hzvlqzph.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wsupmtcl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ytvexfim.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2enjyxijm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mtonsznl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vadusgsb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sfaycfwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjsipjxe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tpotevkf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kjhwzahe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhegvugo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mimynuxj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ppbnpvtf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fjepbclm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ydvnfupj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yvcpxxex.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nideheuc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2azdrmzqr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ovdeafiv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lemlguqd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gcoqfnqx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2avbsmwsh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2yequyxag.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qrthgksx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gdtkjvhv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hcmmfabc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ofakpjdi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2msyqymgl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qcbobndm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmhxjdqu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2tkveczxb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tlmidupm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2utnolwij.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcovgdxc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xkevkpbp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2pgqvgvax.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jzjryzpn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sduwcqyr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eeartydt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tazffyec.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wcdbhtxy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dohhhmiu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gupbkzho.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2opvcwndh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2etxyyjtd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjgmfpef.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nhiursfq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2eltkdqbm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dmjtwcaf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fbseqmrf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kxikdgas.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rwmasfrk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wymfzexg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rppqjbns.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kxgcazqa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ismkubzz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ovukimlh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2txmrkawi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pngpyoue.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ahekwnpi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kueehqqz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mxiuazxo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tssalwrx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vpnzwtir.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yygovakg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mqqkmfss.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2osqdckzo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2darviuws.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2gjibjclz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gjascyjx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uhesjqlb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rlmpelix.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hftkkcvv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zpbbjbzf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mopoqsjr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ipyoyzqz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czsefxtu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ggxaxoqc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mjqnyeax.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vtdmdlln.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wctiofdq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2obhcxkop.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uxnkdkwd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2acohayth.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jbikpwvr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2svdscjbu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wkzimebw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bmpaiqqs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fmlefdla.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yhxpsavq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2efeovcon.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2axwosqsa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dmtgvaro.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tocytkks.html


<!-- 参考信息 -->