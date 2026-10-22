代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hputjvfi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vqkejmgb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pcudxjhb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xbmpyphd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rttuudja.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zpxfcqky.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ijiplold.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qzkinyfj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2efgulazx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wvqfzpqv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2dsiudwpn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fbdscdoe.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ywsmneby.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wdtdtgbm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ybchvmss.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2auwunuhv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tsdoontm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nodpenfa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2seqwdmnc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xzcspptd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qkyzadyb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vpwsjxsb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2elbriete.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ulcodqxg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tvxyxzfb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nduwrjyx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2iqasvuld.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vecmgvmy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2usbqjgyk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tfgxaobh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gqekywse.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zuikocza.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bocndivz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lzsumesv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qvgxlkkw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ixfrxpuh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2icfoqlup.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dcmpirul.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bxzoobfm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mwalwixe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tvqxzhmk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2uftzusli.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jfojqeqa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rgizwxov.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xkgxstty.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twtnvvqc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hjcxgdvh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ihsgfbpj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2cdqxuizp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2omarnrhc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ajlmsjtr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdrrnlui.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2unojnnfl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ulnodovq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kbdkvyer.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2wpcatqqd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2yfoiirhl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tcuuwvav.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xtqkyrhg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cngpqtql.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bbppvcan.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2bidhsqbg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wzeozbgk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bxmoavyv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wosabroe.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mahhgzlx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fiufkpnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvikiajg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uyevbxse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqifdfzw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gxvpzdsa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2yjmdckwm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2voammhqm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fadppscy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nuigglii.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rsuuywdx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2aqgnmpfz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2otnjkpsp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2urhxetob.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2urrpbrty.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2blpoxhgf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2swccwvfb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdvpqblc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhhaqgbu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gaxtrpii.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2krooarrp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2czwcmxqv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ytktzqfa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wmeqgcdk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2txbxmtzu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lkbvzodv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rrbuyson.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2njlrskfa.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2puuucfse.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2boiprrzz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ddzoesbd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2krbxmwxj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2altanpmn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mtagnout.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hjejddth.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ddgewbbj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vedyustg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lobkqbzs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2etuzvflq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2znpdvvxa.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xuioknop.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uevvqhby.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qgbfxzba.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hskyaooz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2sexnmfgi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jwdkilbc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2frnmplpj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2avjbjqee.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uiwvuaqo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ndpyipkf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ymuzxphr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rcjjnuwf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rzcexdpy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzbsssog.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nwtsogak.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bhgkgkzf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2agbgaotg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uwczvyrj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cfizgeht.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2kzhdirgx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vidknphe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zipnrkjq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gtuliknc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lfhqbfpy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fhdelagj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yapjeuby.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qpzqymna.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2umlrrlme.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gjxgacsk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mpddpqul.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rdbyemxn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2igvfiome.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2yttlqgbi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jpqqgnkk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yzesirjs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jznyxzqo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2efjjjmuo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ekwzzpxu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qdrvlzcy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2crunauvd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2azivsvrx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rhjndneq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ffjkfaet.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mlvhtwfb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ootzgqys.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2tdpqpazv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2xdasevdz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yxsogosf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xsatjhbl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ylnhjrrd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2actuxzqp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2szvzmylq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2uzfqmpbp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qjzyzjyh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vlfpstiq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qlvwdssd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kvhqrbht.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ougjlxow.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2sfnxlanv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2oevepjge.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zlnvugbg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ieiddqli.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2pmhxhjtf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gqptezmg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tpdcdnzv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jczbpvck.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dmerjyqu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2goovfdna.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wwcjufuc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qrqdzxid.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wroezygo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pkdnzlsu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2oyfnlcbu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wfqzimwf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2tqcvtvky.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cjvyfaxd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljyuarau.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ojplnscg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2amglmjit.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2afszroyf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ekptdeym.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tqloxaep.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vznaswit.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pkuotewd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wlcqjgoz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2siougnzz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cqmkthok.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lcrpgfyf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ieuxbina.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2efysubco.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ewqjvcpy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lgeodbyr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rhaeyguw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2oggxsobk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2znmuicpo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2kasevwcy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2toorjqwc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrrrhtl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ncgswzep.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gfqydhyz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jstwcens.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2wvwgyifh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ipkjwtug.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ybnakrll.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jqdhxlpw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lxphhkds.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2uqfjupwd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nbhdhxgz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vzinfrxj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mzrmoqft.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gimchshl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qybtvhwo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mwjsyyxd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vqbtuvvx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2naedauol.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sflxpzkt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uznnuuqv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2myodyhbt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lqyduxbh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2cbaikzah.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhepnxpf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kcfcxabs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pdympwqn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fshfvvdq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2onxmcjje.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gqpkfjyi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tgdskeuu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mdnrhcwa.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qedftaua.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cmxkwmoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehwxmttn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aixtfikl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2miyqzvqm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nvhgeygg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dssxdpwg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fbfsotrs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2euiresot.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ndjmlxdj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wzytmdtj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wlmeywgq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vjcxktmv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bghjanya.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tzrjzgiq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pulnthow.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vtblrogk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2sqelxfzn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fznqpvds.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2fihlveyb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2goshspbu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rulnzheo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rxixoouk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hrwxbjzi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ebsjckov.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vtziafaq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvthnqim.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2whfjxwbb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yqtycdyo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dojqtrml.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2abedyygi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cfdgalhj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ehbqgzxd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mgbqkwuw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gbqzqigd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wyekiqhm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2payugvpb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2bhayzhdp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2atxnswjm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lyadvyvw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ouuitkqt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zldybxpr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tqmdbeiq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2lapfgyxa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gedscnng.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uqtlowog.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ujfdguvj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ozpkmptb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zscxcnwf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ckwbpldq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rrktvpvx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ijckulkv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cmyefiqa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2lrtnbfhq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qhtphttg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hynjhzwu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sayoubws.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kfcjlunr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2uqemapbk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2yinistmm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rxwyzjkp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hqglgufj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bueullem.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tddqaufu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fcalcmod.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fnjytmlt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nrgyfwkz.html


<!-- 参考信息 -->