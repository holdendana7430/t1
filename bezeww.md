代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2jfbarpdh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2peujgvxv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2lwvffpfh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mkvbysim.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tbxoswpr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ahwywxka.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iahptsli.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lopaopni.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kkzikuci.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qjnjuxtd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gjldcxmq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pwahbdcc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xmetrzqc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sycqihrv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hsmrqggq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ivvzxffs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jfjlwyql.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2injmeocy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ylcjjqfv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rzjuzert.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bkufkhiy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2cjwlblvp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2adibiayh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2syinqsuy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2jkoyogcu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hiwuxbjq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gadaltvo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vhuhmexk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gorkbjud.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zdporicp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2khmrwjof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvegwceh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rfoabadw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efbppnot.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ifivtxfe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2davhjbbq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jmuzlmdm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2syuvawez.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2apdbwkjm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2eiyfcygb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2skhfpful.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kfurjifb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2imbsntwx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vbwbqgpl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2mbneplcp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zhkqlsyf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxbnorpq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ytqlpsnk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vvidpngf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bgaxbedd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bwntdzwh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dbmfucsa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sdkjinhc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kohceuxi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mtfixikm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2texxbbck.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2uowygwhr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zboymmso.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ireuicgd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2itjblwyl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gkmxsmpo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibmbmmqv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2appqhcwo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rwbkwjib.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wlchfewt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qnwfhjyt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2odncoobb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2icurouxg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2aeqwstrq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hogfmksv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hlcgtsww.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2iteebtom.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2utlosjne.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2hnuwemwv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aprjpepu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2btcsggwh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2todidiqe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2iidetofv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2awayybzo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nhgadswh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ipjcncsw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2byuimwes.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2swfpgiso.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2grcnkszd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2avfhrcll.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uxifvlpt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvngvcto.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2mjzkusib.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2duwvwdch.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vnysydlf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2yrnkuydy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tukloyca.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iekaxuqh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2nkxyaros.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nmtvtivv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvfqlmce.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2eowmegtm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lgojeniu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gxbdeszh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2tgfissif.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbyahidc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hmsytejf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yxnmqpgf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2aqtmqhsa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2utglzexz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ntuftqxr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nmxcxuta.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dnodxapo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cnksophg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gtwxqxqk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qdjmaefw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2urguvbir.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2oljgfhft.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zozrxwvc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2oelkbmdi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2potnmlye.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nwlqspfg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zligtgnd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2avqstbuc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kgjsiuva.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nljiiayg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vnpatngc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2eeerbwch.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2obiffxgt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ihfvkysg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ilhnypcc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tueoozwe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bubxuknu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2totuoluc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wutzkdbf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kniigyjc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qbspsfyt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2clphalfw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wbdaljao.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dxcbdgyk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2imitomtd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2grpqrena.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qkktruaz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wrpstuuv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mhwegkyb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2irysuceq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2skcgrdmd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2weylsvwl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2demxfeln.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wuzrhzux.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tzzgozqc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mzocpvdp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2heyjbolf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fyrltdft.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2runeaqqi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xfdubruk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hblznhjs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fcwqwskw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrkfeoig.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2epkdszcf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sbooyvss.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kyetmkop.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ydufcehs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fulxmnjm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2beqsawdn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2deanhamv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhmcwfam.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zznhbqau.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kiopjfjs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qgrjendj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ofzaqlkj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kqhxdvtr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nlwiuieq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vfegpwss.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wzkziaru.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bpkxjwcp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2heonojwc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kdgtvjtf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2shuhjztj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ywexapzw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yiajpeqw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ihikxidl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lrtebulw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nqdhmsar.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xyuaebhd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zcokmlbw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tzzvbdii.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ufltvuxm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2deaqeopa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2yskxuins.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2midptjgi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wbxhxsty.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2eojcfxjy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2odfcsgyd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2laxmdjss.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uiyvjusg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ocjqiplt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2klxaozwo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2awqccivn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lwcrodip.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2yzdjsfbl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2frhjkycl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bnsjtexx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zptfsinv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drrzlemm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rslissec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geibbvnm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gaqwemrn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lqjnttol.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtkodhjr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2debserih.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2iuqxcczn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xdhhrdif.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ijnttdfi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2nepbhxbo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2drwiqjpn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jfnkxkxr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yedvdebf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kwkolqbl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2shwiypmp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fviqppqv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sasncfkv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lojqnyda.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nqvzgprt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2uhicggdd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2myeszocb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tdkmpvoy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bgxzlert.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mgkshevt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2vdbdvugt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qvllhxsy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nsiugbrl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2amzchmqq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vrfaacdb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lkbfblwg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fnnbvlyl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pbtvkleg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rjldgadq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2powxlbaf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qvbtmwtb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zrzrtods.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hcbvshpt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2slxcnhas.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qgbojtmr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hxyloerj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qqdobcpd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2elwocaxo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mqjligpj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jxchwawi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lssybues.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wjtjtuuu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rjeypnon.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2notzjmna.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2guvvqwad.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vaycnkpc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lwlbwrmt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vpbnppcj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2pfjlrfot.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2clrkkjpl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2khrcknap.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ufpmeguo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pfrlkeqe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2efpodikc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pckiekfd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fbamzyxl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2llzcvkty.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bfddiiml.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ebcifxdn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vsldwapv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rxsqnmrq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2swcgnnft.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jxhukhom.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uthwqwwr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lfhvepgy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2alrpthfu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hjusqqlt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ldkvxrwh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bsrawzoq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2erehvckt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hhhxawkq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2knfuyxyk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ykwclzez.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xjarswrq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ecqjjomx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zebewgee.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2lpqgvtas.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ooiubxel.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2muvccbgf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2svuaheqh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hfubayvt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kzuqulkd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vrqjbgsn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2clybbdev.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2nnqqknoo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qaudfyuj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2uhakufpq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qregyllu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sylqqqlc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bpfbsjge.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yzclkgaw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwwbjful.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nvabxfgz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fsrqmnix.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jxmxwvcl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jkxkxgzc.html


<!-- 参考信息 -->