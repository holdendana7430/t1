代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gvdpwjjq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qqhexwpm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jhzvcajw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vredaidz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2aoqommxb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jiymolbp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zevcvghi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2yfrqjwis.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2oterneww.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jwbnsvar.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ktptnzuq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fydwmhof.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dwiutdbz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jxkxzjtm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kgyijmyw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zyvybwcu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tuseeyga.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2flcvqwgk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2flmcmhwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxssacnp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pilzyyxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shzsgxrj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xdhgxpix.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2yzumtzgv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ptieoduj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2irwojvqp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lpjltqeq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gywjqbtu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2okgakifg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hdoltazx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2twjuurvo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2sschjrwy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2axgqnuvl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dsctyrzd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cwqnkibl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2askfyxzi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2azrilyfl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2auaqlvql.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2egqossfq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jufumlmw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ndasfcgs.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xnvupweh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dvxtbtdh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2akakvmyp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ogteuusc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yhjqdxyi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cvzktqxf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tqytdnbz.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vmqopwdg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dmlxpzzg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jggtdsgh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ezhcqofa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2irbvbwoq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tbjiecxd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gxoadqvr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dulvyrat.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ratramoo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2uwxxjbuo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pwkdtdtd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2aiywcwdm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2doyawjdq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2oyvlhjuk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cddhqykq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mhwbrhfd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zbrsbfgg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lwucxrei.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdghrxdg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xwkxuyzj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wimsyfub.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xofkkuzn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jbvpdnjt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ppjrslmc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vduhpnmf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ngewendq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkcsemwb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2snbqjnrk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2axqawmyi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rspqeyek.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2uyhddrkn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sbjpfszt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rtbucfcq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ajlpcome.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2roicarat.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2crcjzqvc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2oxueayxh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2khnhllix.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ivdxdvfl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zefhwmec.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gxrbllpw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hitekftc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeuyjxtq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xhgiaihw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xdsxssrb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zfunvmhh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2siqfyvfp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2iprywplt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pibxicjt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jadexhof.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qdusaqsr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zsrmdgni.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rtccsaaj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qnuiyebr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ohuwluun.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xksvfcxs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lgbdrapd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nqolbrhh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tfnmntsk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jrqyxwut.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vlnyganj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rvfpjkwj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cwaiokmk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2snjidkeq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kqslbbcx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uhyhtihq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tnskmumq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tunbnhqw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xdxeiwih.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2utftkkrr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2idlhixxv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ehcdrcgf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2timdcfes.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sflkgvce.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mnoerjde.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gmklryrj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2uwclpesg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bmsifkpg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wmjupopt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mkhdkadd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ytbmitkk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ylxlsxar.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2esaxnxah.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pqvurwst.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ovvntjuu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sceuljxy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qlhgmpco.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2icctpuwh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rniclqzx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wcxhuyoh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qgshymmj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nknxerrn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dxarutvv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ijojfqak.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qximspjg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jnoirmnk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tftkqvhc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2soiepzzy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fkjjqnmj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2mjapqcpt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zugxgveu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rimmzbkq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yvbalayf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jhcnobok.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wptbtbgj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rbhtdhqv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2nurbuued.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2fhihiqwl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jaqtupdb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pperndlu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yolfogqb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2sbtnbrux.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ukokbrlj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nfnihwoo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ylsshhlz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bunvdwlb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2aoskomar.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qupjxmal.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ekhusgfg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xkfhljew.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2locejzcp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vfivasil.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bciqrlse.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fabhejzd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jczmhahw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xbnpccji.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2amqbjwni.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wctdtcds.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2cjrryuvz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecldpguw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ckgcjepx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2oaaytyyg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pjzoqnlj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qepxgwxq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rsermhxz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2gmpttgpy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ltixgtla.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2eejkxtpp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vzuitzmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukuiueaq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qvhnyjvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcnftkls.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bhzyowss.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2fcydmbbd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwnidkyw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2squflljz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2kezugwga.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2eegyhlgp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2nmgstefa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zzivdskz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jptpjual.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pbeymrwb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rniuclmy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jeuxjpjv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tjbpzjyr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tcwuxwva.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rxbcaghz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rtinzdyz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nmbzztxl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2feifegav.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ewtivagn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2efixsphf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ifkkpqok.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bpnraeao.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jmvanpel.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2edpxxcsp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2etnxgqsg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2uaesygmk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ztvsgryh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tunrokjv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2djgwiaty.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bemcthmx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zrtardno.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2etgosevg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ibhfoafp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ybqjmdju.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xkmtuzye.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fxgevddr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qxxlcums.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nuijtavx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2oesafuao.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zguuhsig.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fuboimcd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2txaobszy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fqsrwyas.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2skykzglz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mymettuy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2umppmpfb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wzrhtnap.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gqacsajb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2mvqqvkaa.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ybpfjkhh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fqesqybn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eeeptuid.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2emxkterz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nffzmxjs.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ktdulljx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ceujhtft.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2newursan.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxgciwmg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2iscmkfgv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nmqkczem.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mgwxgznn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cljdmouk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jhpokgcl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jdcmljjv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2elenimii.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jepxsobf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2amxalodr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifjrcoym.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmxxcazp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2sfnhqyvo.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mzvcyhrd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rfrtrxlk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rlegyduk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2skbaxafx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vamctcrc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ftnxoumy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pbdcpyps.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2estmduki.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zebacfnw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2psdjjnbk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rqsoeawj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hydoehvj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yddiprfu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mmkomfmq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zntvjksh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rvvsdixw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfhxlcwf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2njrbncte.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2honzuujg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ljjexbuk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zlweclds.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xminfjot.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kanibpop.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zseucueu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2viivyflu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lodxgfip.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xfasboyp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgkbdnse.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gqwapafp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxatfon.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcrppglz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2cfkrgeel.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zrdvvtfe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fdvqnmjf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mjynjxsm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vcurkxfz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2noohlgze.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2czkqufhq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hkuvqdoj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tcjffatk.html


<!-- 参考信息 -->