代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3oddznuyo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zflelblt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tulitvrr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wnvjrzkq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pjjwugnj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sqwyzytm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3pwfwzytj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3etfozbpw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3tznvrywf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3etsamnzy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3mrjfyyap.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3aqjfjqtb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pafmgccx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qoxjaffq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jvjdthxf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ucvpqjmq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lciiauoo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3piaowjuh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zivikoot.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3phalxiqv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3yyzniuml.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3svxkyeex.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3pyovowyy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3aexwkrti.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3cxorrkuk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3htefucjv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3impmfkbp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3effzxyrx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yqwietae.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wkwhvpde.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ayfzjasb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ziocucbm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gbcucvhc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgznetgz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yvehgtrg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3frsuoqlc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3foflyrzy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fldlmcrf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hkllcutg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qjxfdsip.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fnnsdbhb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fjnqvour.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3isllelza.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ubixdyty.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xoldhdet.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3umkfumko.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrrcbrvs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xrhumvvz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3eloljerj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lgccxedq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rdhiwlsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpgbosbf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vfxldetc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxoqblfc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xoqddipe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3uzdiozwl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kpvzvozz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nmxikqtq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3uqkqsjtb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ldmuiuhz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zezhxpwm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lswryteq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3cgysjcsm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rnagzbes.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ogxjgbjv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3thutxeuz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ccstipbc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3avzqmpok.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3itznitdr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pbjxzshv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3khrhfabq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uktlrfjj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ypwwgnix.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uvkptkld.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3guxlryjk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rnbkacfy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vhavsxyt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tppmlikj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wtesagrx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lgmyqvsk.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sxwzvnga.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3oofwcpyn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dxetjdog.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zkfqktjq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dxzewbri.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3afpwdfqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dwrlxodb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jiurgdih.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xjuikjnq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ilmzbuqa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cgqfobdx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3asjwidak.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dvdnakwn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3iyqptant.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bytnrmfk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vpxmyndr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yhcyyuxq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tsticoqc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gsliczrb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eawrtadg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rmdxgytr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bsgifnlg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hqlgrlyh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3osbzuhls.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rqqgdfvd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ctognrlx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3brdamwrb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ivngugvd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wftmdvhy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wmmtoida.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qcqejpav.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3eoorrrtq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bnjtmcvq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kiylaavo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qtqzojiq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zkrmiqpt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mxtwdbvc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hwblacvf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kehdhllg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rhdeitmj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3txglxnlm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3scoexdsr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbfcawvx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3irsvfmlt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lizqikld.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vzridbyx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3emltqlbe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3inieiprg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xhftdbhf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xybdqdla.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3adoowrvq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvdlpvql.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3sbqayeoq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wwqwnnab.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qkfpmgmr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tfkpdeoy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cqzmejiw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ovcsrabb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ynrtuzvu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3azikfkre.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cbruquia.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3vgouqwkc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3czvjwhfg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3aegebvrn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zwpnuhhm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3nxdplxpm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ssuzbutg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3uoepqwgz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jlljrocn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dnngdlvm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cvthoydg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3afhnwxqg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rdsmpmqf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fiwnjeof.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mckzknfd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3eqjelyls.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3byimkeko.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pqolhidx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sbrifsjy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fqrfgpii.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nbxetddc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hjzfqsqs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3adshjwvr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3msammqfn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3opvbhrbn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3valitxya.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tvxachuk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ffjgkhnz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hyulfuaw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ojvbydcq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hzszjqjo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vtikuqru.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hbbqujve.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3neyecndn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rnczmvsj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3axayyyyl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3emoxcdxa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hptjpvzc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ojncmbol.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wacgyven.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lsfcdwem.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhyfqcex.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3yucodekk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fnunemvo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3eglndsjm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rfqzgszf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nhzctfjc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dsdxtrfy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vupyfina.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lodrqzwl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nflbtdym.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ajxvvoio.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3imhxjmrr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xarlfqfr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cuxgocyb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3uyydagqz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ghggpbwl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3iaxymbco.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kyhpoatp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3njqupxgv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vmdpxuee.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3meuoutkk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3auksvmjq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vcrqzjst.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3docfkcdg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3twllpqwk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vlbdxuvo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3eaitvqhv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jiqjaeat.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hkzkphrs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lfhrykrq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jijqgjvu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3sqhbnzya.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xakxpqoq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vmsntzit.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jbueogap.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tqwkodbq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jfbayxml.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qlfjxzuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odadfsca.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lfgybyiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhyofpkh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtcxxveg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3emndegqy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3voetnubd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cjyiofgw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cejgmdne.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zucaulaw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vkcswuhc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ellbjybl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fowsqgtc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qliykkxx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvtwzujb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wjmerpoy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3smdvkpdy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dzdimfac.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3htcsocit.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3oireisma.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pnzdxmhx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kdbxvhsq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gkikafnq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kzoubwxd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aqgmtrid.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ijfgujff.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ngcgwulu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zdcpaivj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ykopfzhc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ybdctcag.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cuwwfzxp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ecwhwmnw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yefgddox.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tbhjgfpn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ddfkzihs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vtcpacyk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bhxkxyhc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dfrwzcjm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gbwcgetz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eyjklmpw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3uuirpflk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wkuivdiz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhihsft.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3arwuoycj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cbljsvuj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vfjsmyza.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lpiverah.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rwvfahwj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bngwicsu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qkvstzud.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bqkwddpi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qxhocuiz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jnbxxfkt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3omuhzvra.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xduupwdi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kmyjvbrx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zsmpkkpo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3evouozua.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yfnzbgyx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3svlcdegw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3odptndon.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ngqekhtn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bkdxequs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ymvbzshc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qvrdkkyu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zkeqrbbx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3swucerva.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3orutzfhd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3lqgvadid.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uaqguxjx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3thbpdnyd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3spsguzzj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tqxhanjn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3icejnbqn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nybejhen.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bktrkcdo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gofopfzg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3oozxtoea.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kmlvsnva.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3utwbxqih.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tjdzpdwp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3engglztb.html


<!-- 参考信息 -->