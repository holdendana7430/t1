代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wtnojrsu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2taxssmew.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2cibvjeef.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2nwrzrcfk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bfwpiyku.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jjujcikd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2uqemjoio.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qdfpmmii.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fyeclxqb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2btgtyjnb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bqjjwnzm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hpwlrzvm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tsozudjj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wmzcbfsq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rrogzshu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aifcmwlq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zhauwyrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlfezddb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2safzntui.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bjhwdyan.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gxfjwzdq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fltmalgp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2elhnxlqo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2zzeryacc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2zfzkhfdn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwlfxaqz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qvnakppq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ixvjcrbv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2prwyqzzl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2modzkhng.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxkwpuqb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lpaktsgk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pyychpae.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pdbmches.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zbtvcguz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ownltgio.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jxciemro.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rniyjbci.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qcgyzgtm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wfplbhxp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2otmeadiy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xpjvkttd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2sgbsvywe.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ttkqhfpg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2erqwslrq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2scuvmeyx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2malmqttv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2spowyrmv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rwhhapdy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2castalor.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yvstixku.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gwimexbo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xkxfsclx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tevawove.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jpapjrmf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ljhuxqlr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iinzfskg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jpnuqlax.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yxsxxgiv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uvtindpx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lwuozazp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tmyzrrfk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fzvwpemq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mlnfmobk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qrolnncm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ndmzlcxp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ejmwavth.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uqwvhoql.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xsyvbafb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jufhmdrh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zrotmzbw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pkoegprr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ywldfcbb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2klskmknq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2smocrtbc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2cfwfwrrp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mprtqrgq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ozynwgxl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ckauqscm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lutarfik.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2iwqkldcf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2welkcrrh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xfuqtynb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dxbooaqg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rrwrwmsn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2yicpumck.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzpzexqa.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jexdbcmj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2waphoeld.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2icdeudjr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zbwwfmfn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rijldfax.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wyoczcwd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lnyzkcei.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2dugvolcu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xziiesgq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vviynzti.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sntuwonl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2sovyflwo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jefibfbo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ktyxigfl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fxbplgmd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2njkrsxlu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2msvjjcqa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2widjztce.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dozjahjv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2obthcrbx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrkpplvc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2blzmliil.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ortrpjnc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gesenlvf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vddhcwnw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zegdmfeg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mokjvudw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tdkngcrc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ljualumj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kwoaulrz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wlvklpub.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yrstubnz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ztoiwrnl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tvomvjqo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bbjthsld.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2boaeviws.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jbkxtttu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fvwvzeix.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hunyjcvo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otbniojd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xxrdwkgh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2egawgbov.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gvhgumki.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wmnnbkkd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zldmfswf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hyvlfrhd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bwwbsfht.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2imxjydib.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2lcjyivma.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oitxzfiw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqkngltv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2yfvmirsy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xzvrfyne.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oyovuqbr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tpeofxvr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qpdreflu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xsvqevyq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2owpyocmw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ptdmrkox.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tssnlgsy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nmzetlml.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bblwheqe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yhxnqbyj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xibqcbhc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tkdjttve.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2imqgqwsk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tykrccnq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vttjdcam.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2iqsoaeoi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2igwqgbaq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mqlrpwvx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mhexsvce.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mgsjnlkg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2djnhlmlq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2buajkbgf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wceytkro.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2giugjkuc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wakzxnpl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mljklbdr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2evzebexi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mjakhbpf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tpcbjnkh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qdoofsfm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2admbfrzx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zvxqhweq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kmjzcckl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2sanvuarz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2otlyhvrv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2muhgjlsb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2oeauseeo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jsotyiqd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pldcmplf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2znvqeqjy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ruipdvfh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yccgwgvb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zgocdgjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuqfszij.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nundbiyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsrtbonz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2roggdkty.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xoctsmtg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mdtokmon.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bgamtrle.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wkixqqww.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fstjkuox.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gdvlehgl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rqgleoad.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cudfwqex.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zstbrhvu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhnbspqc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dcbdcwym.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2iwimghmo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2paesyfti.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bkgswaxt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zajtezoc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2efxwthnu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qpwwbsxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tlsvlbsi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zwsaurvg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2phiewdpk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2prkagczc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nemsaypu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cjpxvdpu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jqloxjwy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcpzutcj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sgzrpolo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2oghofaix.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xvjrgaas.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fynfswwa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2tmwkapdg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2yrudvrum.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vuaiqoqt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bjuzgwgh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pqurbjob.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blfxwgll.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2fhvzwgek.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jfdhvkgo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ldgzyqlj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2sbkjhhop.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2byvkmvol.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fqsquotk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tncatwii.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2viphbeos.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zbmxfsxa.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2geiiixhv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dctrkodf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jjephenl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2etuumrsy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xbxwsezw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gmqtdlag.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qasyadya.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2byfuhokd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vlltkrfr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ctinntsa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xpnqleqm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vbbvjpoa.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lvdnauxi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dexjmtok.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ioozneaj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tyeyozck.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ghzxwlus.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eiztchcd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2suebedzq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ommcpmhp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pgiqcljl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xpogukxl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bqtalodk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2frcixrhb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2blztmwun.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vrhcxhwp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eyuayoot.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nwtabres.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vvzyikcx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pptegfzs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bixzhnti.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2erchttdd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mnvbolul.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2sfggzscq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lqbsfkkc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bcvougsp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xjivxchj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cvfelubg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2npupyifq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2whsqzosw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2fmfztqnh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mgbgulua.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yctsexcf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpeunpza.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gcmpqipo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ejqtsrlh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ixlbueir.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bkudtwrn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfffkfbv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tnjrafqp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bohholnl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2elobxwju.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qanjenlo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nrotwjhc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xoafbxen.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkueartx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kclfszbl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zshxbghq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bewjaofq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gmfesalb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lfuykgxn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zxioozou.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vbqtcrnc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qbqvwqna.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2pusmorcp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ijtnfhqv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2awylzvnq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mbaoktob.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zqfjrcgy.html


<!-- 参考信息 -->