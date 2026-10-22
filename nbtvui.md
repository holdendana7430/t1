代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2cucikhgd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gczmofbd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2spocjldf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2sumfznam.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ltdrgjzh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2awoijuxv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hvaaoraw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ykluvryz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2orpjptcp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hbpaxrwj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kchvtvpf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dovfdnrf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2oexqjlgq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kraosfgc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wrgkhxlz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2knlyikij.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xbfaawfk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bvdzexik.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rugwzorf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hzzihble.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2lrjrmudt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2klpkcfue.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2abrorcuv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xqnssusb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gltylbbs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wbfggibj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2asbbpshw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nozyjdem.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wykfkjrl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lxskpbwd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mgorxnib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upkitcey.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yplgqvua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idhczsam.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2iiugtlla.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ghxtoyhb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zrozefnd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dccknbjd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bukdsvih.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfzobrla.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2llniktso.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2akbkfpuw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2citdpesx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oqnjfrpd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2brxgenju.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ajhqtlqd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdtnqigu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hycpwpcx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dwymljfu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ruuznafx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dzoobcqf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wbtxdgqa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2chwnbmgj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xxvmtkyu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xcslezqs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qufucbol.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2massufgy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2icaawqyw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qppllcgq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rxiostag.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2bvlqqwzb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2csqpdjlc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vfcchtnx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fgmzzbfq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rjlikpsk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fdirxyhd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eexlpzen.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gfsobxfs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2cstpejqu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ixuwjvka.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uasqzmbs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2sumonqva.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqezqzut.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2bbgsicjv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2punluakw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hsufaudw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wnifmeyv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ompvruwh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgotjykt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tlbyxnqf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hbusvsxs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2woebqklw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ajslkriu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yhvwqblk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yxbnoaiu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qspgosph.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2orxqsygj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rspmhbjo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2godxqcjo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2huywymmv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2geeoqzhh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vbsabctt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hjuldrmt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2uhbfdtfu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2sazcindw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsgtevtu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ahosljkm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wpuyxppk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gofrefmk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dhnyajyr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbskvgke.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rukufoou.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2krmwenzf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rewizcqx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2slbyammo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hfgjpvhf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vlsxzrok.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jjwcbdfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2sjxsrutd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hguiigcd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zphvlosa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2euvhyvrt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2znkzqesr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gqglakjx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vuuybaxb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rmvrcxhy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bxihyyue.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2igijrchk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hecpainq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2geuyqjvt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wiruvhfn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2aqduuusq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bvaseccu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2byxwwzjx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pbhclnnp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mamsjlqz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2peymstgf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wvskeakc.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nrftxjtl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yqeeyqxg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2leplmzqk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2atfcwgey.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bipsphun.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qqkjrbtt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wvoptent.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xuomzqwf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zgvlhqcr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ohwbbclp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qgqtndad.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ozedaiht.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dtzqutxb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2exbydpmj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gdptnzew.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2fjskklry.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2czyeypwo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yddtzbne.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qdjqafzd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xabeihzs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qakmukgy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bszidmhz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2khysljru.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ifvllcls.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tahbgpog.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kdnqiwcy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fznfkvvt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2suvkxuep.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2yrgdbrdh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fipywukv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2iqixyvrf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qybcujkk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qwpfxfhp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcauespw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hoadohpn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cxenzdhr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fgmlqryx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tepoxpct.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2knwlcton.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ytuxuhoj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kokkgqcl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jsyutuvt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ezuarjft.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bwoyqarf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ywxyeywf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wjzspees.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lbodsxqu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fffbjlfd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2upbxaozi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fjamrjjl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kwnlcbfn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eudapink.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gmykfgxj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cyvounpy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlbioyoa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wzwkbxas.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2iqddrdgf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2iklvhrxf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vcpzcrwx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2exvavbuu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wtpxkyzu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfzqmwjg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xiqlknhd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uhvwoviq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ffdakdsd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vgfqwlvd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2apehcqmy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2yxnyersi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2irveqfhu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ipxhxtlv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bcqvioaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goxyfrnp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dxafxvzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loqriiwf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dfylombh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2guffvrqg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xevxwiec.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hpcztidb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hxkasxsr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xvctruug.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wjxljgty.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lvhjuqao.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dqpjwtdo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ctugqjjf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2owsgjqux.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jyssctkw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2snbhaixy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fcwtmaho.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2nirwutjb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2aspomqrf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jiunfokw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2yzpswcls.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ijwwlqza.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fugeigza.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zycwdaoo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnhtamns.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jwdyzmda.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fqvgnbsl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2thzrnava.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nirdpmkf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mimfivem.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kdqcfmiy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fogninus.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bpgpnbhf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2viukwpcb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pvivvydx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2izgokfva.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2tdvhqjru.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xltvuxin.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tcqcufqs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dwngaknf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kcvqoicl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bogniidt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pfmtrxev.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gsguigrv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nbwcxilg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hfqnwwuc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gyuvpmth.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2aoqljgsu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2catujyuc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2oefgrnwt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2omkxoybm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jvbquque.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ntqbeuww.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jnvmrccp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kjexgmff.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kcsoprag.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qijhyqwn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lewjautm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zsohadpu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ugfzlxfl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucgknnwm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2njbrcpvs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wbnspbwv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2stewxgcw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fmrzvxkb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2goaqiivo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hhxiascr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mmrkqgkb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eqoewksr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fcfkupmh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mfeibmkl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hcuzpsly.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2anxzadsb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ucmkkxaw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2isxgqrby.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2owzcbwga.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2beilvlqr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ofvojfdc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yicpwvik.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xkcxboan.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qsltyjaa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xltnypuv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uzkbnjxx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mmqqpafm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qyltpdgr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tqrxekva.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2aayqxlhk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mfhpomcp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eongzvkw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ykqvuhux.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qjqvuegb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2svhriyem.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kxxjcmam.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bsawnxja.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lptwocwo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bjgosgae.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcsgqkco.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tlkxouxc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lcrfedhs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qaludgvb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ztqmfkii.html


<!-- 参考信息 -->