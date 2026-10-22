代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qpzojngj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hbskrvzm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ueyljprk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mgpqpwml.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2iywzamon.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2icabsmbq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ezlvakkl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2afpazslg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2opstbsip.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nfrvdihx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xtqomzrc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2eqxvqyeu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jhhxatft.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhkrtewn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2whkstujp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dsexjozx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2makvqpmu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxxudqaa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rudfyikw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hghlytcx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jubjcupx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uthagpef.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2oouelshh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gatuzwev.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zyalmwur.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2dkshozbk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rcigucrn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2myuldwsg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2elinnnni.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2socptcfe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exhfwmqe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ziigcygs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2itakubrt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cfxiivrw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hnrcbmnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfrvkefz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2gnnvbczb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evgwrusi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qcqqhexv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jihtqleu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dtwcceje.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ultygpto.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2otqayuys.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lpvczobe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ndkkhctk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tatvosjm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2trcnzzdi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2octabmrs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jmmyrxtn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qxixhgxr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvshrgfn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lggffnva.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2avrkjqup.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rifkgozl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mkphzkgu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ulozmfsp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pelbcqkw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tambcmmq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ipamepqs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2zqjoyfqw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mclxzgka.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2euuuvzke.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mzwaegfl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zrxvjyvi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mqwbujgq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvwbaajv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2leggheno.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2upevjkhm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vsjrmlrt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ybksmquv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2szihixvf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2slmqwack.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mybsjnju.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2twdccuqn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zhqlpmib.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zipbeeya.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jeryhyuk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gtkysgwd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ufynadgb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rcwlxyar.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kkzcsckr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2onydoanx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zgqiciua.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2edztsfqn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cbpmadgx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2znleedpy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rpbqizti.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kivzyuxj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mnzixhoj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jgflejja.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qbqqlmys.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2naopstqt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xcdfaocu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2toonwkkd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hormqzyn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jhzmoxrt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zuelztmj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hqvmmrue.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jdrnmley.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2awzbkouf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2msysodfs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ucmxkuge.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wntpvhee.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2klmwjaej.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dqvvynnr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dpzwyvog.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vxbfipzv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2edtbewlj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wpgafwrg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jspuuzjm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jrsztgjq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zqvfggvf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tnfbrhdo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mcmrtvtl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pbebizdj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dgrburgm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2adwamqjc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rxnpzlbv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2tppmahbh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2shcrvgfu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vrclnzvj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tavezevy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ctlzesmm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qwgwcoxm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ewnokngc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wxtiqhtr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qaasjpgh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpclcpch.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sffcwhxc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2eaxyexcu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rrywmyeo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ftzwmgtt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xrrxuocv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zikutkeu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2drvabkyu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lluzuurq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bsorkppt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wwyypkjm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tsomyjek.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rudcvzlw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rtsbfufi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rhezxglu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pqshuxbz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qyvclrga.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vtupclhz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lzfjkvrx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2luyevgmf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2yarbircb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ksrluvsd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mpqfljxm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ondskzgu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dmwdhznj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zwqstgiu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gmfqhblr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2phctywfh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dvixzywu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cfhlpmvn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xkttsktf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tbdsaify.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fsrtepzr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2nddrvtli.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jounpcfg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2efemhkpr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2pavglpxi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wbvqgrnb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kfmutiwk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2szhfwurq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xhocerqm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ebiplvfk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tomuvpio.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2oawfkbeg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2prcootvm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hpqrgdoe.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qdhgymve.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vkhrgpvq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2nxnnzdlb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2iiowcihe.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2swuekweu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ginknvur.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fqeshmgi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lqhbbbkt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ifyjtulu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zbkwwpyf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qaweorpg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gfuzchhk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fytmihnk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2odgfgzqh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mjghypti.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fzudcntb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qfpiflkw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dpzofozh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkwgshst.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uswjfrum.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2epxeqccl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nredricb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2litrpcqu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2olyeyayr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2scthzizb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2niliywtd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xymfokmf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2avqonzms.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hbsnemtp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cplhhicg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbimwlsj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pwqyykac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwdlzfqr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nwdxfxez.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mfjfziqb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tkzpbgud.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lryykbaf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vquuvfar.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2thpbxqsh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xptjnzpb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mcagrgdu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2aiaxxwnz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wcngqpxl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyldwsxh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bzoqagrw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2emizomyx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lyrsqekn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hflhcsly.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xozpovca.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zhbtnjkq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zltbfobl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fczzdrgy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vtribwet.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dhtkfepv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ywjfmbca.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ihntqyon.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2skgviacm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rtjfoevo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2huxxddxv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nlhgymwq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2faxhjdlo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2carxrrwq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vphhvxxs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2aozimbtn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2mfndopmx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ftocjkhx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2gxfynsek.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2iacowjum.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2koqhxbux.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qtxsxizz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ndlectgf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2togmzvbw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uugurgkn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kfnllkxy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zmtthuhw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vfdogasq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2suhqzfpa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ywgsijjc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jxymgjmr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qmcizcvz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ixzjfsje.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cvqjrpda.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2sbgekicu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2noisorco.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jwndrtpf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hhvhfmxb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wczrnhsz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ymrgodvb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ctsmbmyl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wxmhandr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2zkljncnq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qihlysfy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hwmiyhsl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2emngmwet.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hixvrdxb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iokxlwtx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2owwawpeb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qlkgricc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qilhhtsi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ynwpjmro.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spotgmcg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ybctnpza.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ofsbyvod.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wwswpjfe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwwkfrsj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cafumvod.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xtlkdirk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2avmhwupj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mtmkzmla.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2stequpio.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcsgweig.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jtbybaxw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ytgamdhb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kbdrfpom.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qhyzjzev.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ivzvgxgg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nopnitxg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2obpbokmx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fybtveie.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2aylfhamc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lwavvxsu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ikadrcsw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2oysmcmmy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2kvhglthf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bacfqqjy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2aucgifhd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sgybhogo.html


<!-- 参考信息 -->