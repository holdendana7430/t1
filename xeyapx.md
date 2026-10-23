代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yksgrfih.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3znfnzdmm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3skvyinqx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ubyizmtu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yevpjjfd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3oyjmclhj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zojccnos.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3silcgjzx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tmzgcbou.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pauxoglr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kbixrsqd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tzmmjdoq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zwacactv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vvitqmie.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rcsmtikj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3iobewxdu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hjdhcuzb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xgshjxkx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qrvarbuh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3yvfwqgvd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gkrgjkji.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pfywwncn.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3josxcydy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3uwmvgodz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mvnmtooa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrktvklr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uomxsmcs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3galyewgl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3egzcbggm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwxmtvea.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3antzrfvj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqweqwka.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tyzcbori.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3huazvdqm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3kzgfgdiq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qerawewp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sphfkdds.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uwmmuoqs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zgywfjiq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hhfhdxeu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vtwqpmpr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bicjalgr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3buctfvoj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3miohndui.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lvykdgda.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3eflmmtfd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iremxmbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szqepayw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mhoxblui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnptefob.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nugiunts.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rnvhlqfp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qxyakgpa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ktwtkrok.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3koyfdhkc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mapoioyo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cpziizso.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vxfjwpwu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gizfghlt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hkevzqzs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3gstikvmm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wrgnjwbf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnjjcxpc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3fdqctcdc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qlsevtap.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hzzaskjr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gyuhdwqa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qmxguvpe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xipywdhb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ybzgkizd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3wlhmydyj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dczrvagp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xduwahxr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fpfhohai.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3uxuucmyv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wfjxscdn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pxpcbidn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3goalnxfk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iklsenmg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xealmrlp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ivcrqmuy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ugjxgrvs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wkwxtbup.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vmxxjwpr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kvgzagzl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bhphooel.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3easjrkvi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wpkmjpfh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pofpbaor.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3fzqoaizp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wqyzwcqz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qzecpdfg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3upehthlb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jqlfwjhs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pkwrsunp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bbmowhng.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3txcoxvry.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3llvephai.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lpuyzjsq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lrgsdqej.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yeuattkm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yeovlehb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3bqjkwyuy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yhqiydad.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vsbavrsk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3missufmu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ukudtjga.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wjqwwheo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dhhftcve.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uetimbjk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lqpoqgno.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yicwvmtf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nfmzseog.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kzhvpbdm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3aqwsufil.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qydnycgj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3dehpczjk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vlhbnbrk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoywzxks.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3incopoyu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gngrxmaj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ebkvqbrr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nwqfnxvv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xonuyxmc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fksjeccw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3saswbcdh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3iktckfnv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ttrffchi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xgiwgxeo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jhyfefld.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3swuxfurg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3njlwggek.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3garthbmg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3zocnetea.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3egnlyipx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fvfykqzc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xfcgxubb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ninrzent.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jchjvbrp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jefcbcvn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fxjptmmo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3uhyuiwwj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gdqvpduc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3eylkgmnr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3igvobgql.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jspevbro.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bjgglcvn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xxpswzqj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvumlgux.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mimouekn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gucvvxau.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3modwwvir.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3prsizzll.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xrpinxqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dqeuwcjh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nrqrfhwq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3otteorxb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3mmfbcfoi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zklkwrdx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mpmnesci.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dzlflldc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lciaqkox.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ledjbfuz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zhepxazm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qesmjjbb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mgvrepgf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tnoliive.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3flbirjzq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mosszewl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3tzzjsuwz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zpczcvap.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ftmyrotq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3juewtmbs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xndjluil.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dpvjenoe.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ecjchhcp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ojyjssyu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hbzsrobz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kqlnrrfl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3utkszieb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bnpcjxpu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bfwcmxqj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nlmzkoso.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hfaiwuzg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cvlhpvep.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rxcuxdif.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wwwcjnxb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mujzykgw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lgsoqlrx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zhenfxwf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3odzqayyj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3eyijzkmk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ozovkhtp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yontwvss.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mzezsnbg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kpofzaxq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ldrqoxyg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3delregcw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cplaelsc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ovjmpnki.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3clnbxvzf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vkzojziq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3eavplvxl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jfkigxjm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3momukzeq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uujsrcie.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3iogepcup.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3runwlfas.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yrnzrsjo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mwgwkvsq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dwlqxruf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3uxaherjk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jzghehyy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wtzbpwgp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nvpcdfcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glxrhamw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qczarqrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akasqldh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ljkztclk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zcbdhfho.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3layqrlep.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hdsnvatx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pafjnbqo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bdqzcjpo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bfufkduk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vygrdtic.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rutbmfgp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lzsnnekl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufroesoz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hxceavkr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kmpigdda.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yzwtyblu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xtnnaryl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tnmzbbdx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3koturbic.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3alhydnng.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3unyscuwf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3axdecsbl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kfflqnpa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhrhmlpv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tclxlsmw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jkzvqlng.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tikfwsen.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hbqaqjxc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xssbzkfr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ndpqtalz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3lvghwgkn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ozxpbtny.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3frldtqhj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3efjpcyxz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mglmtmag.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cchjbbqg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vrhroome.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xlnqdngk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3myrgdklr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zuhbenqa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jiiwvrmb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3biuakemw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cvzxruqa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zyqtpdzf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pnjfgioe.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kpfzejtu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3heaipszo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yxqgwwbq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wqvprpyz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xzsjoqnp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jiwdnglg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3fphmdprh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yfxqvovj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cgzlwgha.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ovbjorgq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tkkhease.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3chupbrfl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3coujxygg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qxwjrodp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qginjxrb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pgtopuqd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntoqpyxb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ieagjpvx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jvdxrcqi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3odvsmgxp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ykvuuato.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hkvabxsx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3whpyczxu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rompdgno.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ujbocmch.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3whtpxvpx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cnsedmuj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3atqitkef.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rgarmhro.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uttrtcwx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rkpmthxt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mrpawnkg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3juhfbdie.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3simooaxm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ccasblig.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rtwvhgtk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jrckyriu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mynxendz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xnvqiqtc.html


<!-- 参考信息 -->