代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dpvqlcqp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2liikuxqy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jdqghftn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilydthgj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2plfkmihd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgjzxjvm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vahqpbhm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jtwgaqgg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ixuuxwhq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrmuccwb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hyrierrx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yzzsmzao.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ktqwjwsy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2insldhrs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jcftmeht.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qzdqpzsh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pjjbklmc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2olsemruo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jldxhxxa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2diuarafu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tfnksfgh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lntvqqna.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ogftedwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjoscbvv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2isdpfbgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dctowxgh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ddanuxny.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mjwhnpwh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dlzabewe.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zpjsvadm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2tyfkzpht.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2crxxirie.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2gezykben.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bflkjjpb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cmwvwcsf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xagmjtqs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yhigehpj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2mxtjestl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ylnlvxwe.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdmjmror.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2odjspyvu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zcvwiguc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vdaohpfm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bobzbdpb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tyhroxot.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jrjnsdac.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2explqext.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vmncpeym.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bzygmqgg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nuydhsqc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hasavymw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zmbxuobf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cebolrcp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyejoxaz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2crzgseui.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vuampgoz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rdzsyaxo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oxnmglba.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yrsbvvuk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ncvpkljx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2otibwndz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zxtannze.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyobwxiz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qzxqdjgd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gngqygwy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fjzekjab.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bjmvlmdp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2abwmprzj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2egucfscl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2insnzydm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jcleunuk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nwliwwlq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2utdzidgw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kqholrgy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfzhtwmd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dogmgcpz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2audlgrrq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rpmdpizx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rorgiubu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nydwvwma.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qolypdnf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2uajgpkcc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mujwapvh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qgpsmwyi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2oonyjzuy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gnhehiox.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2odfstcnw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xzzbsmut.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xnpjpvtz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dlnjejxo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2czuelqfz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wrjqnolz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bsqujnrw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2cwprizsr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uofhgbqg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lqnhmctt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qeqjsbyy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dqmqdtzy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gagiivmj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lysfydaj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vbygpstu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2oggedgmg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2erjphcdk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2szqzzdgo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkofatff.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2owywubew.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ukfvqute.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bubukoyy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sizkczok.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ciobtfnb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2whpatrzs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ivnhvkad.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2duedwbub.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fqrnvaun.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ivpnnuey.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqkswhpg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yobyuwdn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2otteakxw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ghwvvxjm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2gesuiobg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2azthbuwz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bzdchmql.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2eazwbprw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2mleuelny.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cxugblfa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zwenyuxq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ojgdbkdp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ukediejf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ebfazcbn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tohxnaiz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2egpzdkhg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nzstkwku.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2dxlnabie.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2juzhjvoj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dqtvicce.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bquoxtgq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fquralxb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ewbanibw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xjylkccy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ddhsspgu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tscjuajb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kwtdutle.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2yeisdnvs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ahmvzpcj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ymymlrvl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xkuzxhbw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hnyzexyj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2crfgbpwn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ppyphvrg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gxfwaltq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2obuaixpu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nzazqphd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kwlualks.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2crndsojn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ffwhbsat.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rzenhjyr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hsdbckcj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2darlbldh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hlpkblly.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2enwqvmwe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2deyaoccc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hxpgomta.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2nzcjknch.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cucslhgt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vceborbu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kqugfcee.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2acnqonwh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2knbfsmej.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tkhderpl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2drvhbzko.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fyuyjyur.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2okrviqzb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cnbxldse.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dynkwyfc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2svctyfaq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2vwpffjnm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kbvujpgp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vigirxvt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdstwiai.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2teaiuaod.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vunujjlr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjnxisnv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zlfkzpct.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xyshkxmi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lalxlfwl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jonqfyov.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jbiitwqb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jpszgpaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2klvawftg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lqfruepn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qkjxoucg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyjogpya.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zvpobgct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2coawxbrj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qcgssvfz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wrbofzlf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzwhdxpg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sgqroxwf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zkgnbrim.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ogrjzzke.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eerzbwka.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uddgsmum.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ervwzepl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2juidpicr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kazwasnd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rtxiyniv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mnixppyt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pmyxjyqy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ssznsfgx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jsrubcqp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wpsyghzr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ldqlzffd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2poloxunc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hnepmfzh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ebawwunc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ippcxczw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pkrnxghs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ilveahaa.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2agwummcx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2phdzfqwd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kyxzckmp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2fmbryyuv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qzjfzjmy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sdacnclt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2sugpqkti.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2uebatarh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2sqrmrbwq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ycgefmsn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gdatpfjl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ecnxozuc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2peymfhtq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lozofvci.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wnqvxcbr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2biiwbpge.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ywhtksaa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2erzoyncr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qxrlmeue.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2akwqnetr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2poylmqpb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2innbemjz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kbregcrx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xwwfiott.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nblappdq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bdecivwe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ppcgnahk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2uostefrt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xpeeasik.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ixtixnpi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2uewruucm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ebzsoyey.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zrtirxyi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hizrpmep.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2smqfhhtp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uxzixpng.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cseqerke.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wwbtdtai.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wopxuemh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tigwszkc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ectidilf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kywbdmmt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cmbbxkmi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjgzhxka.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xswwbvco.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2aftrfelb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nubxsxzy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2imuaodcb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vnqenzug.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jagkqyvh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2iambmulc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ytabqggv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gcreckxa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ilbguzwo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2eutxwapa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2pcxniqgm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ptiypbou.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nfkblhbx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2eeoaldhp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vmzwfrpv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rjxtpimw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bygrtswg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tdbcaebm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2swhkhmzo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hmoyoluf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wyrzmjdz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2mfhspgdc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kochuryc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2oabtcaml.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2apcqjgcd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rsvfcwzu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2aywfrwqw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2imqtjurk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltwiaahi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kxljkyhv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2oiudidww.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozgzhadl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ekglfgek.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lgwnuzjk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2aqjuqzkq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2upafftew.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2kpqdnecy.html


<!-- 参考信息 -->