代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zprbjneb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrsjysmk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2widbyhvj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jlfincla.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2oufcnrba.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bszlsdkn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2yrhsjyxf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gtecuxry.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2inrjlaxe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2moqxquyd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2feejetfd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nkstvwmh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mdjtpgzq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2iyqaqnjn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dfgbhwku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkxefhjn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zhcoldcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfxpwjby.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xadxfkqo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2qixuldhq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kxeacsdg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lhbcrbnp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zklvjsuo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cqlwgkdn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ehepgcfv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zavphtvi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vxpsxeua.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2liywuxii.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vkwkcpdh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2frtavlqs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqqqeobe.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gklbcruu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2shinmywq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2sgwhweap.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bttfytsf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mmfdxsup.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2kpimmxdw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2sriqqtkd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uhjdkoqc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2baxfwqyn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2efpxalno.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rodhboyt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cqfyxifj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2pwdolaxe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gzohtgtu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jehofwtu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ekiarufz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dcvkxtpi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cgfjdqku.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2uzblcavp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fgrhfpya.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qkwqrevy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jvjekbir.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vwvygcjk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vbkuirth.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bvootvrr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwizqshk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gojakpbo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2emdkjfby.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bkpggmrc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ixedfpwi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2omtuqxib.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cnqcmkhs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2msefbqtr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uaztxpdb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fbkkbepu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nndlpwvj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lbzwzfee.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pehsdtei.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2apdjcdkf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2yblckkek.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hzymfpmo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2optgqaho.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ttwvtszf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jtfdksrs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cgwexkif.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mxfehuoh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xgbusiyk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2elaedzwk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lglbldbu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2aehejapx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vtpfhwes.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qkwgekwm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uvwaickb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jehfprab.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wgegdndw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bhvbzply.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lctnmliy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2iwhxzzim.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vnzzbdym.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mttbchzt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ucxvumqb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mvwhnrng.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bnswlytj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kambbyni.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vtiuwdnf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2admgvngw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kxrbuala.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ockykfnf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2aepawxnb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2clssqdsf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kmxnksdh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ysyxjrgk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mluhgfmr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yamabvul.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2cbseplyc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2hesvqzxf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2oaqlqowp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wgsepgug.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ufxddtoz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2sayykcrh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yuokwyby.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fvctdlph.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vntchjzk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ixmrjanb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2orvlvomi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zozowgnm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hfzoetcr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iraqgnrk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2miwjqeey.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2msgdbyei.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lvkblpoq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jmeaqgmg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2yvlnnpjm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2xejxdjej.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mmuuutgf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ksrobqwh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rjxsmkah.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2iqwczhtg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kwnvyszq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2obhshkzi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2foxplhsv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cwrjfiak.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2auishbkm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mtrplecl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zhiqbmdy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jkkfgciz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hilzgbhp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2owphgtzr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ajorckyv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xwqhytdn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hhiyrqgb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ggopdunj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tkaezksm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kgvbvakm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvaucxqv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rjcuvsfl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tiltowou.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jalegffp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jtndnkqv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fjrxapal.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fnmdqjgl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zmwvtcux.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2borcgsao.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2yjytjdwo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qhxzwoja.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tfrknyaw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wpwwksbz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2smbxmjma.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dbcqqrsj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vydkhrqz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bcbcgadd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fflvqivo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nqpfkkzy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2huklpjjq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wulpwope.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qrggqmiu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gqllqtgf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2noxwrefs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pbyzrsuk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wkovnxqw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2aqtpdyrs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2txlcpcro.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pfnqqreb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2emipdaan.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ytewnjid.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bsplwopl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jkaupftq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mxjbslir.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rambzryd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ltpnklvu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cvykpvxo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wboethkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcsvsmls.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2llgjlmuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szvhmqrq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zeuijxke.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tqraugcw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2lmkwwzmv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wobqvtlh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wweyehve.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cmvsynri.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2apdnefay.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wblsbcgw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2urvjaeuc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pgdmtowi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ucpwtadd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bkdypfuj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ztjdziep.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2abcgrfgr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rufbljlv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pxuytzqk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cqzrlgwu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ufdckkwg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hcndofek.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ycmsrdhl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2njftaguy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiwyzveg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wobuapmb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wzhprjjk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yvcntjfg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wsymwwif.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ddkrlmlo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rvhhafyg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pfrbjksf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ksccgevl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2picfrnhq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2atnpuwfy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mfjcjpdi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2uiqylbpx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nmqlynaq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2prlhkjgv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2rbvgdhlg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fywpckwo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mlcinerr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vulxowtx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jpwnrujy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xxxlqelh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wsyjuwtj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2mpskzfli.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lkwxjwun.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pntyqwqs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2eawzawpr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ngjyyduu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xhxpxmzl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fjswrxqy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2mbfkfuba.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hfuhhiet.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ypyftzrt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zxirlyeh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tkmujjhx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wlartlzn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yorrzvwq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2avmrkkpr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gtotfjec.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2skzcnlbe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nkumeiyr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lbdlwxqd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vhwjqtrn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qhesaopg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nflhqxtt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yunrujye.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zddbkiaq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2omauraxt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sfsqmnpx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fwewkdss.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2izorynag.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nqasmcbm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2aecagzeg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fgzumyqd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lglvehnk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zskhwqyy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2fzcfvqrz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vmfqzuyq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ygzibstj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2luktvmhd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hiddikwf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dzouqtns.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qmzhhmho.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2anprszkh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2sxeclbrr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2oqumrbzc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hauujsrn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2nwtaihsd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rlohznyo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ndmiornx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hlqncswm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ixtfgmdn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2onloyujy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lrebtjrn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ltfybpig.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dqxakszs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qpexwkvv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tjlbovpa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2klzfabiz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xfnhdfld.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqenukch.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fjpvwdtz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sugrxacg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ukwjavfd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lwjzfhmk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mmlggdym.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2itlolftg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2oclemieo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ayfijpvc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vireelji.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2yynynfuq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2iglvfrti.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2yqxcomio.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2fzwxzqtw.html


<!-- 参考信息 -->