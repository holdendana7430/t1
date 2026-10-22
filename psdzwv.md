代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ermtdizh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2soljdjpb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2aknfdtre.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2pyezlefe.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rkycugeb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zftmeozh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2oufwifvh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gegxfwgo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2aiooputt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mhzebzll.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tqhysmeh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2odhfvuhy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nmciticn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnzuafnq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qfnnhujm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2iitmmcul.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ygmkobng.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mdvcedij.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fpuhiiep.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2csmexfye.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2btvjdafr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hotxsvzi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajuwxqkq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aiawkcme.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zkezfptw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2stgypvtv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xhfncyzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhlzbojl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cyeytxpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btfkuhak.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qqhklvok.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iczcouyf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2addhnoop.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dfokvlxo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mzjmymoi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fkjmnrxo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cjznwpsz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2djzyjfau.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2levhwlig.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ereqrrmu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2spmlcjhp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wjlgxrth.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwqgohnq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vypkzili.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sihcenkw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hrvzkdvr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cqfoqihx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2evrurvyu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ecywfllx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dgshemwt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fjavyhep.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2apfqrpqv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ijncvqcz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lyaqldbd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pxeqvlpq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uxvicenp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uqnuihfn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2iydkwhtt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tytwvahh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2miqclryn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qwjpenuf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2rnxsjumd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jqsvdcfs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqxoqhrm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2npabbzet.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2owrznfof.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2trxyumrc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rlfmycqi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gpttrsuu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2cnahffyt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2slvwlaha.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fbsntrov.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xfsyepms.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lxhrokau.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ridessvg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oewhlgyr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pjfwkdxg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dptbtrhn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nsqvgzra.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2twuguduv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hbjqpmut.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hpnkuglk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uvyeguyo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2emkgspxf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rezwkptp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xguegezl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bndvkqiy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2kkzomnnv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ybrmbkxr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zaarppyu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hcuikate.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2njhgttrl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2gnscwpny.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wvavuphx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2efnkwpfk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qzoyjsfs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2aunqxjtz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jylmheqr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxvtqjct.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rbkiyqlz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zcnyneqq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2iycuuqic.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cyemglyc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ynyqqzib.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qzuvditb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cwfkmpaz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nizlhrpt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tptlbzpa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kjpmuwmz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2etjlqsnp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jhbzekwi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mqptzmvl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wyianmoe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kppxztsl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qhivscql.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dcbwawej.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qbhmfxtu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qswmbkhd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2argovvfy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivfxinul.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2aluoxxop.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pykhszaf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ouraextq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vxzquygx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2chfqoveb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tzbxsovo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2iuhzbefq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2puhnaxat.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vvdbwyyu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tohyeyru.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fmayojie.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eqdxfogk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bkarifgj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hvqnzuia.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2reyexpcj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ckyrbibd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2thoyoonh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2nqkabsbe.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2bseuobwj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2onieigpa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tmmhjker.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kalnehco.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lbireyxn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qxuazurh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sgqqvioi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mbipfmtq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mafolgju.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qkflzaxs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2gjcployi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zontuwvj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ersmgvvw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ewjfibga.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2gzxmiasd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cvsddbhd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2rcirundl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hspqxcdl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ulooeulh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lrvavkdq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mhdyqeva.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ogsqezld.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ylfhemqv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tcgggntg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wymzgybp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qndsmsml.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xsopwyjf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vjhphpdk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xsuknnan.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ivfhfymr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2txpcruuy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2khoxqhwk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tgnzbbdf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nshxptol.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rcohnbme.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lwyefptn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gajlrllz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rjwqnpir.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2djfluxqe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2sksvxjkc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2klbzsddg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2umqlnhtm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2afnkpgaq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2baufyepx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pvoiwnra.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gqpxxdjb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2stutdbhr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fjprzbkw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ajbkoirs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2cytxeifx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gfoukkji.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vdkpbuwo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gilfwrlw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wehiykfr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2gnicscmj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2btdmrtns.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zktvnqvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcprlxsn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ojhulimd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cefeffom.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sifwmjrh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kixazcwi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2enjvycze.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tyntjfkl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tpjbjdne.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zvdciyec.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2lrkahwte.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pjsxkddf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qevbmkud.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sadayktd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xajmiwpp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pbdouxgv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fpykgzxk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2oyoaunqt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pcujmgel.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2bbfvnuop.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2spgrhiiv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ncucxwfh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ekiimsvc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2aatdrjaj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2legnlhqg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xjbxbkyo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2epqwgace.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pwmwzhmy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yuwzmdkj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fkacdgfr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2axqdhsib.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2thwrmnsr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hqtzemvv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gjjdidhe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2urjdysgn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bbvscbzz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mkldtxbk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2xknmfpyb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gkzqrsep.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ypphrkli.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2blkszwuy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fxceauzn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2iknrsuls.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ywhidwcm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bdouudwr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lvfkyqlg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2skbuzmpi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vnkhieen.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2tnwxypcy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eihbugxq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lptdbqis.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ledjpwbz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2aicitldn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jerwjsrf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gdjywxbr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lobfcier.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2htbkbtwb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qecefaqn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2azhefycd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2txzbpiuy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aedqdnkl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2omnsbrbe.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wsouhcss.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jsbpccsi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ijgatfnc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2evkerbtx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aczqugxd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2whhpmnvi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hcahzuwb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nsahisxn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tihagfoi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzeiyyvv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ncnbahwk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dzzxftys.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rxwgxzqi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gyyglasz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sjwoyiqm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fntoaazs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jjoydtjl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mhooqcbq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gbsbplrb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2twecngtr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zgflvinv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2adelnofl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jaafavpp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gjbbnvpb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2clsnyxhh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qwgkpabe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jcjpifzi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2knckddxs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqutawnx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kmwrrlsf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yxztbobn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2edpzwzke.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zjgrahaq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mfirmlcl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2koviinzd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vmzpkhke.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2svcxlhqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dzguvoqc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gukzrypm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nhreciaq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2niiayjfr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2szwgaodd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2shfzofym.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jzggspvy.html


<!-- 参考信息 -->