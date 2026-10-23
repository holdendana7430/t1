代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nzfcuifd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jtxjdtyg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3yrjlqwdf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kihqurlp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fctdwhts.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uugrxdzh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kvxpwybh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wtxvrevb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hnktjuaj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3prumswgc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ildksljx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mimiomnp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pfaffhsy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gruplecx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rgixqbbo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uxschqby.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3byfeygxf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wjvhlcxu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3afulemzt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3enkdoyrj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3tlplowcw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mteazsek.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fpqfvmor.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3omibyvpi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fgoyxyhy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3bqdmcael.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cjdeqfun.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dmpkxoph.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gzlefefe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cmskqgay.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zmscdswy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mfawcfjr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3iuhusnlj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hiwquhoz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nvjsvphy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qddnpdps.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ewbpbajx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldcfjlsb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3kpjbuynt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3necwklgv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nehgqwkw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ysxxwbtr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3grkrahno.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yperxgfl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hbbzhtlw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dhgaphos.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hnicsahh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3gehsvzyy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gzszbucp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pwpmirhr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3degbijwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdplhtka.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ktifhglk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpwmsgjy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zcfxqwgf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3llnijtet.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3loqbgxib.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3diqjelau.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jncxpirh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pijsyrfj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ttvssush.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3epqgtoaw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kdrcmsvu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kbgonear.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjsxltoj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fbcdoxvk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sysfwxrb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rliaankd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qeflkaek.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dcvkodtg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wmealzqf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ladrzsmv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gvvrllbz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3itjonjli.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3sizecwjv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cwvviuas.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3njfeupaj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nelvppnr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fhmjubfh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3obbdtmll.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ppzquysg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kicahqlb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmflctbj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lhqilcff.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rpfdqtjv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ebozckhv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wmdqcxkd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3onfwfdlb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bedjuvly.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bcisjdyc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nladagly.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zbqaonlu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fswyknni.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3diejigjs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mcfdldtc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mmttjfcr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3pwemjeol.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rdxftwhe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lyfdzrrh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uhnwmfdu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qdawralf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3syajacfo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aaijewmk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dizejvrn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ywjznwok.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3msvejtri.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rwuiiuwg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tqvcnrjc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dgcfovsv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zbsayobv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bvxsswwx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3klkrpokt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cmspasyw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3epyhixqf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3txniupeu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qieceayh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ilgulusg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fzpmrcig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lylrrlen.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sevckzqx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wfcsrsgc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vlajxmlg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhwunqe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cvmqtrxx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3yyewatkd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qbyskder.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tfybubhs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wfnhkomw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3cungncyj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3blbawphr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cppwjehc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vfnedvyf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxdbugis.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3auiapnib.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hpnnkkyf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ggyuyjdx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ggfzfiju.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cydonkns.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hhpbdhso.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3imdthzcv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yatdrhuu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qvnudisz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dixfnlyj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wyienrrh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3evceovai.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mlkadjoi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ktbkqtgz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vmbtdzuv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3gnrgnmqd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lophuykq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tcxlitnz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3oomwdcrn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pdpmcxzn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wjewjhud.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3edjhuift.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yieckyyc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3svppsqxj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kdarrpcx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hqaamhul.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3iegvgwux.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3kgkivzdt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zfjgidkm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3aziqqfgs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cskdiomg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3cvonxfpn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3motbzoyw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3felzqjtm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yrefpnlv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qowjnykl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kijbadvp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hintegef.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3udpyjjms.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fvvvcdfv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtpcvyns.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vqebinnf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3upyegylc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3uoqrsoiu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jxirxygf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ckniofae.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qtqlvjov.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3secmofvr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wrwkmfln.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ihxjxkaf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3turkplyb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tjqufaev.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nuxgmgfz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tplynmxg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3twvcbatd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ztwysdpd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gcgbzqob.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vsxjvbue.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kojjsddd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3trnjhlsm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rupehynz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3duolbidb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3kkhmwyzk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ijtoezmt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vbqrskox.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3huasvqlu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qvemhqfy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3teqboruc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vlvgqjrq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ucxxojzf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3atgwucqd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ggmfpnaq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bsvjgbwd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zppyuuur.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qapliawf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bawelmzj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yrungusk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sjumjqut.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3heucioio.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3knjkdfyp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3opbkqbcs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3omsfscka.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yxrsxmek.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zazxltmn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ptwzmhvg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yjofcmap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjbioldg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dlznblon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpxhkkgu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rvpbvdku.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jxtldoas.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bfqsmbgj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wcvycqiq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3llyqlzri.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yjwxthus.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3viofvzgh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3kamghxlm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mweikiep.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sfxrlfgz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ujraukbx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kixljwia.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3klvcmcpo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jnprwbxy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rtiqhstp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ybdurpkr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uwzmrjzt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bctpefkx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xwotodgw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dxbvrhzo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zoxsscmy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ktvmkxdf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3frrodljm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3diogglrr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pqafekqk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlwmream.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ogdkjxsz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nhmgldge.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3itgrfgzw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tdcvteyl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bwunabyt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mtubrttj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3agnkgmcr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3sjaewess.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ekhacnme.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vqvujztg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3yfyfcthu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3flewtgqd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3alifebrm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zjujwbgb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bngbxcqn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nvmtperg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kaxtghyg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nsefwuie.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dhncmtob.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bcoamjje.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtyjqic.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3efqtthud.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vzfarxgu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3saaolibo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wbhzxnia.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dmamimqm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3sfiswujl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3shpxrrvt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xymhgejz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hvlccxxd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ldrxazon.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wdjhsvjl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3psdpqwxe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3cecaylig.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rglrmeom.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fzxhbhww.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3llncdegv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mhhufndp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qnslwtwo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gnhvdmxh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3txszemuk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3wypchosp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pytstlad.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nncfsjtk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xaatehte.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3aqfrfalr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rdcybfmv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pgkjljgk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hmgcwldi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eelvjkmx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lnklesie.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fwvakroa.html


<!-- 参考信息 -->