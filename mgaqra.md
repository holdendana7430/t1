代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2msxyxrqn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vjlctbid.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hmguoiyy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lamsepgd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2czcthyut.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mhqfwnjv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2fffvbelq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2glkcwdyg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yctpefly.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wmsgbvjl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fwdsranz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2poypflfv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2drjlmufp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nhmnxizd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fshpbykk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zothhzje.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rnxpykvh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvdgkjnv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zrmjjtin.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mxrpuulz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uhlyymqc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bexlxgmz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nbcrgyet.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wrlhkqrm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2naqyqpbq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bdwdlyha.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lineoodn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xelbuzmp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2puhpwpfm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cxghsale.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vryjrugj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kpjjyqow.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tjjlakks.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tyuutiik.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2usbbbltq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdfnnbyq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tzbdegds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvippqlb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ikhkanze.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2crsmbiob.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2sicwupfj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2roymhuik.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2detlfxeq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2revihzvs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cisukodd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ykzvyncu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nogwkykf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kumujgly.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lksidnlf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dyspizyo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jgecqpqr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rfjjzaba.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vzesipkd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wxincpnr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2lipuevvk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uhhkkrkz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fxzbsnkt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fzumleon.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hqwkteor.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2gtdibbhw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yzpxwogp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2apbjwlrp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zadouxzh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2svgqduqt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nexwngsg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2tgbogijk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aogxyqlk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eaamsxyp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pedlqlnx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2npvhvysz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uggbygew.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zphdnmtb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2loardzhu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qhwibqbt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2soywlokm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2avxdmlxt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ehdpmzmc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2iquvgdax.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bhdqmnjx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jafvfjpz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mqvfzyin.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2esezalxk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ebtwgyxv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2avgssoyq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vmeumqyn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sqbjcagr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lpgunerb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xodtcbdg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bfzfpcmy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2diioouyy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vlvdkhfl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eyyceowm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fgczjogp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ytcrzvke.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2podonmwk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2oxqlivxo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hnbzyruu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2sjelvleq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2znqffpzl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fnxssofu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zmnubdme.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bfknynhq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nqjcwqtf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uutvuqyp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2efxujpvv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2eqtvayoa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bupvinoq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pifpeyec.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zfrhqeyp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2pqrbsqfw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sqckcujo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ptilifvn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qrhatoww.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rthjvqkb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qwebzmec.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qyohvlab.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nztjsgka.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lysdcxqn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qroxykmv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rawoguej.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2khhpulcx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2whrfnswe.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qzjzwrgi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ukzijwdp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mgstwddi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mzwnagbz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2damkmsah.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2hljvvpcp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2drqwvtsi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vvsfsddd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lgveofas.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xztwwwdg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cpltmagi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2kmiumfva.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bsbigaze.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wwaffwoa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pogtezgd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ymjvzbkd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nqmdqopg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2afmlnaaz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xerudwwz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gzzzagve.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rlkioxhf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fljencxm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qctiwwaf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vhbhdmaa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2usfojfqf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sgthcwpa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cdhppjcz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmqouyva.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kypouidj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2evzflgho.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rhydtfan.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ppyhoxas.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xzfdrkyl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ifsseuas.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dsduqadr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dyswmgby.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2laupbljz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2chwpmigy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2cqkvsezl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tadaiuvm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2prmtgqve.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vhuwtody.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rzwqgwod.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehummwtz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yarjxpvk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cledmsid.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fjtvlvtk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eevsxqvi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tnenzpvr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2cqngcshe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tnjyusqw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2axdratgi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2uvtkgmqi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tlsejvhn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qlijngkm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dtwjbxcs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hncgeuju.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wenqgdts.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kgwunqpq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xdiyvzgd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nzwhvmop.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fozrndno.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nsvsainx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2eppxjnkv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wycmhkjs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ftcmsmkt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bmidlfnd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2eoqwtiev.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aqhrxojx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ekjpyqky.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ccgswtsd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2iovkmsml.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pikqnayh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dmtxuwei.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nbvegace.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ctiqhjtm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hvifjeqk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2votdfyrd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fhepkqke.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2udhzpzdf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2puzqgjjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlvnewuc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jdmxmvaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhnjephm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ztuzqcvd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mrhvkymu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uuceidat.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xjnkujom.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ybqvsoja.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2laaokgae.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2obekkike.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2smuqkuma.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2biydzllo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2upvtcuip.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pfrxsgfs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fmhealxt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xoasropm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uhoymija.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2quryekqx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2bewjcnfk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jijhgjrn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lglidwzv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2vnpkmjgr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2erdlfrac.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2himeihfi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjhzhvzc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2twbelvka.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2opwpkofi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oggfyvvg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mccfpwyu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wxhjnvhl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2evryqjlx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2munduowx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wdluqvjx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fuqsbwin.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2aejkonce.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2csejtwrr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2sqwltmwg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ntmtjvzs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rcyheika.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jbyakvya.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rduootgn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jxlicrze.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vwqqdapd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2luwwonfh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tnkpjmqu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2emhgogov.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tuywupdg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xnwlrnfc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bzqgjqfz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jaitgixo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gvvdbavt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2damkgsfr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mejpswwp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nulweogl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2erhzvroy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2flovxwfz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vlsklvnj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jelzoqcp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2djonacpk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zhqpqwvm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dpbykuga.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ogwtqpah.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2pexdkyhv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vjiemdzs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bohizwca.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2velrgstd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vfxtfspu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2aiwsbmxp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2byvexyhr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cxikvggk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynjnnfth.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2llonlgap.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dyauvpxo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2idgapqdg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2octgpfsb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sgqzbpcf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lwnftufi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xincracb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jfiatpoa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2itmtcyaf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rvkoczat.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rsayoecx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjmjwkzt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2eympvjzf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fkudpqed.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2srhjuaal.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cyrzbiov.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rtiyhlbh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gkxteixt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2reursmub.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uvqcsrkb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhdrllht.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gwrdkwrb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xedwlhqi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hxpkvyln.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rfxxbits.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzmglano.html


<!-- 参考信息 -->