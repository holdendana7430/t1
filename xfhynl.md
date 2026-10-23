代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3siwwiyzu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hggdikla.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pfnyebth.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wxglfivt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3uwtfrouz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fxzgvhel.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dmupzdla.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rhbjnhoy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rvtfcjeq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovyovcak.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gsfuujiw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iybuncwr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nzfcunes.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gbufljhx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3eeaezlgo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zeheyzna.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sobjyreb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ksqoukbk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ubbdnzin.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3iugpoxuz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3drzqwsbe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3apneywpa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3axjvbmul.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3pvgrpyjm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gogpehac.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dvktiduk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3snbfeupi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sohrgvni.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dlwzdygz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlgwnpiz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zpwhjkvq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tyqeksce.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ihnoieae.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3asllbzzw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pggrrwqf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fuuaeybv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pfpgmsrm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vgaxndla.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gsumxzcy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pchhikgt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lamhnddt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dcphjdmx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqbyqzmz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3aintkjmt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cnbopamr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bkqjrzuc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3blynwxhs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pjhmrulb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fwyrncqq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3sykzaqbu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tlhytkwz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qhnrwncd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yisxgrce.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nffbuazk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zcdwtaqg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ohkcenxn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3lppewamq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3uymazdbk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dppdvxky.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tfwapgce.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qgaeziog.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3knfxdpyd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uhkyumpq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gbjzxkbo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vehvuyuw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nojbnddd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cwzgnmqv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ephwanzk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jgwouqjf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jmsklgti.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qtbdftyt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3otxfedgw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tsmowhcy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zaambryv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3shqgmild.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3otsiacbg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kldnague.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vlekznju.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3yllpotvu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cyqgldds.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yiqxzqlq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jubzctkn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mufbwyds.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lqqfywlb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wnmmlomw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fpdpsuxo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mzcsioon.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kmtlrlqu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3exfeyjyw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dzzjvqfb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3sbphwjne.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cepamuxz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wusdyizr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vdsxgyfq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kyhwecvp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rhvnvgrg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbafpzff.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3oazftbqs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjtmiqc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3loweuffr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xrzjnyjn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vudrkofm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3crmjfwvu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jqozmdcl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3omjvwvwj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kpaeybme.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pgqwfnxj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3tpzgpuux.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fivswpan.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ibstkvxz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tvmcvstk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xvcsjryu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3amzqzdlq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pnpjmwuk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3euztottw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dbhdisac.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fxmwasqf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jyydypsc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irfyxyfm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xdumvuwz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dpmpcjpf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3teoahjor.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kaouwzzv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ccpzxgvv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qackmoqo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jdwtkefy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tjwrzaon.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lbdysqdh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ymcinirt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wtztgowl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fsjcbrhf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kmzzhaoo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3wrjcefvr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zpjjkgav.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3phnkhlga.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qwlqslof.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qriyidqm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3oosihiur.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ljeffubn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lfjswkdt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qinsnvkv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3junbudll.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lygsijkx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3euzzkiey.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gnaheerr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wuxsnudb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dhrruhqg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fjaolcou.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3psbhircb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbfrvyiy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3sunibmto.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rhasgokp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ubwagmzj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wgfhjodo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xshpdvcd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vuzchqyq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fjnbkmui.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3sftlkhpb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3plluhbvq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3juozwdot.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kljgagud.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mmkmayrm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qiugkhpq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ceotfhgk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ukrbkdxc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ckvfqfac.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3fyxddqdf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qvzwirwf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ntpwwgjf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3shrtcwtb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ikymkdvm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jzaenlnq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gfpbujky.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qtofxzfk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qesojaqq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nmuaqqat.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yrtrfhkg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3dbpbspod.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lcyilsgd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xnwyrpbt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xmhhaupi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hxfkqqem.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3smgiydii.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ceshierz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ewwyeqvg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3olbxtaco.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3egxfxfwg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hicfbpyo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3piinrvhi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wafqgaqs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbamgjfz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jswwgpbl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3yfmlqurf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dnletfha.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3sdnhleqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etuswvwp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sfbjvhes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnctbfyf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xsnnzqpa.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3wpzcpapu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsopfigd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3raedtblh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3atjzmept.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wqxqhles.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zloaoyll.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uytoibdi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3otkdrqer.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3guqwjokq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3msrmtgor.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vuitueby.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3wvdcamxd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jqpfhamj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kavixgvs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jpoxopdx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lonpgbpt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ixxsgbfi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nuzyudoe.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ysxntdkl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mthcdyaw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnegjxtw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3teinnghk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zpcixjfw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qvtrkwhb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jbzrqmdo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ncimttye.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3owgbpysq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eqnwumxo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wexcquni.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kmqbtjzg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yguasjee.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3lbzxalmw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lvphrnza.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kuhfhyrl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zxmxtjhc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fowftiog.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mocayoly.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rixlcbky.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kposgtag.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lyjjghtl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3blaxcvak.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wbnlkobs.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bpttkjuj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kbdienin.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gzubkuqi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3crpftciy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uxccbhcg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dszehslo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3fdqbdjyi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lmvvvpaw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qucrdawg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3rjphdstz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jkkzlmgw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3riwuznrh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jwiqupoi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bocmrkoz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gfjzlucx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3awzepknl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pbudfeyy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qvtuasdm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fktcxfqr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lwwungxx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hzersmdc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nucbfdla.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rfsmjqvo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3vuodlpsy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hakssxpi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dtxdumpz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lgqrtwcj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qmvdegwn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ofrboukl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3igvxgutd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kbztulcf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3fqyxnlen.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twdutgsa.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3daktqkzm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eyeibirf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3haziddpx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yezfajqr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cqsqglst.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vmmqrojl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3axchozqb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gcsnuecm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kdxzaleg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mhlyotfs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uhurxokx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3siklwmau.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bndsrcoa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mjilyybc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gtjcxzxr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3akvywiwp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jwndbsxs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tovmnhun.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dlpxqfdz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3drazxviw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3exjrsyei.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ikcdpwtl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prmqkzay.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdhmtxo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohyasjdh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3yahzbazb.html


<!-- 参考信息 -->