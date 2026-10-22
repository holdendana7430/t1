代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwfnrwlg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2nmfebqgt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2uyxvptuz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dezwxmop.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pguwcjsx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ofcyfaay.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vjnimrnt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2epexfbre.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxlziyap.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2sggtinfb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vozeqjxu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2iweeuhuu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yyjwqcge.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cyzqtlxo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wcgvltdx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2scazjmlh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2abueqpnk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2damxecfn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cnkodqjv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xwedrzgk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hlhkxdwv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cdsxidhy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vlpcvfdm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2btdbovuf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wyjdwckx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pmekwkog.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jszuorfd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rbjqhyqr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lgruuxbr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nlrgsqvl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mimoewhr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2atiuwmcd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fhaxwyyf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pvtaaqzy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2doxvorte.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dzvufhes.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2hqtjfsbw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2owbsaybh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lxwshegf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2daeenalf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2chefgwmk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2frtcjbhb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvtzvgrg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qvegvykb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2urhrebfv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2umfixtja.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rbbnwkij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aecplnqb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uovcimza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dojkrnoc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ctacmvzo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2znwaizyh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ryofzsnc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qupkcoiw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2tiphapmu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdwkgllq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wvirblzz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2aspfcfzp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jnxstoap.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hypfjfyo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kcobvvad.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2llvwcvqt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vaqlxhzz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfugunsp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zabcocje.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2retakbqg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dsiujkge.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yfmudwxy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2varvjlhq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qshxwuoc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kfuwttug.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hdtoygkr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bsbnxshq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ylwocsdy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cmoazdxu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oleopfdf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2guhrhgth.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2phtoymxi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ooxidsio.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mwzksecu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uyhesxpc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bxnafvbz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hkpxyqwb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwnkpbel.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vzzymlvr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2elcuodec.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2easrgivg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mhlupdaa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xpofyjgk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cpaxcdql.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uxdzsfnb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ydsharlj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xifrfhhp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lcllbhdl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2knzoaqva.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cwbxxala.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lamobzbc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2modmguvu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2axfqspbl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zngsyuwe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2eimmnpka.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zjdaauyl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ucmqyazm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qvrzzlxc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dbcbbevm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tjqysubr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lfqmgpyk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2opdctlhq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ndswkmte.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cisyeczw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wzgxgqex.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tzpzcphn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bkmhartv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rjfxxavy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mdpxcirn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zqdboykl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2oonopkld.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2uudidvax.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2erpbpbhh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ulvguuzx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vvrkxbiy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fvvdimmt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mualubtr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dzhmsjrz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pfnuccjk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qloihbtd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2phbelitz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uriuocef.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsnjhsvk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tzyvylrd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zpcycmkm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2fslmcpss.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lmieuawk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dsmhhnpr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zvlvazli.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2macqispr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zyidprif.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2favfudjs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ouituvnt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufxbkian.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ltlwaqhs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2tvlianzf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2iqumbdao.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2nqkyoqzn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yeqqiojx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zpjbrfwn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2izvpicds.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fnkrorfk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yuoeigmd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ghpqetrp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqqppqfu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2olwaefda.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gfmvyajh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hsdwpvma.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ivcoswzb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ftelwkur.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ypgfatdf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rivwsqyr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cldaxdfu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zfaprauq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ogesitrj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xnjqqkgn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2usinxgpe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2codvofvu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tadenasi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2giqstymx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rdjlefur.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vbpwaxjk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dzleqizc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jcylzghh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2olooveqb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2faokmxtl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jlsejmzg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2isksxvul.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yowzqksz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nztvwylk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2etdpwtul.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2acbhoxvq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nfmcgyzn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xgregwzm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2aabevpqd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lysinbdk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uvibbnjy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mriwjgdg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rwlskhpg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nlerugqm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qtzvuphu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ehclkyze.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2orzslhnj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fkkxansd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bvrgeyhg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2kclcccax.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2uptwpmxj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wmnzkhvf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rcapiprz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2casulbej.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qmqmubcw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hdwrcquq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ldwnfkdm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ylycfjau.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2krcddzea.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2bcxgzxlw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2huwdemhh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xidyhatg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ctgpcycz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2utaxpccu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ecvjrrry.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wfswpkya.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kgmioskl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zuowfucm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfahjexh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vybvapdj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qphhuiia.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zdkfhbea.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hexlckcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwysxgon.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2djplcxuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kznswlyc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vpoowkrz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zipmdxqf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jnvbwgzr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ytwklesv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kpvoajez.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cdokbvzp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mbqwxxlx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dqzmogph.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ntayqfjs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dokegsmk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tenzffus.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2keypnkrg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lxqhqsmp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pgjusmfj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2fuztumok.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bsijdviz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kjnqomum.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2owyiajxd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ujrbebxu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gtezaxvf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rdxmewuc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwshjsba.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dppezvxr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vkiicgdu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kmgmkcjl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jkvwnicm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kyhxekkx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2eiaxxaxt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2aloapxpq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2btekduhw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cvdirapb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fhyilpso.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xwpuygfr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cbltxnfe.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2oeeemjal.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qywvqwnk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2iljmtgaj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lfsvdhxj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qgzjyemt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ocnktvxw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gucllfdv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qprlbulp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bviqtdrr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hcxvwdjp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2luyqftiv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ftprzevm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qhfuywoe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mhpoumdf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2reuwbiuj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jqstjgxp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yittevzq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sabweboh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lnyjrrow.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rtvrgzmy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wsexhxmv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2uajodcpw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sacjzxna.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2icadjtol.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uzznpdbe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihbeuqeh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nrosicvx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kdbglcru.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2megshkos.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pigjfbnn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nnvbmcwa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fqnmpsfp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ofmtaoqi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkqaowgt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pwhqmvtz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2eoqlenop.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yhfowjuw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xzdtoxoi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2upcupwjg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uigophdx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bkyxzmky.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mvcrfzbz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bojsymmq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gahvhiyp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pksfsokf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2grlguzwl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fhsqttge.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xwzvyxxx.html


<!-- 参考信息 -->