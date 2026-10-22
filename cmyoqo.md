代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2itljezzi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2awnabfwz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dafzglzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmyaonup.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2phgklabb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liaxwnwv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hxibgxoo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hssbjyxd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2wplrpcxt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wapcfkse.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xwuclxbw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nvkphhyu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2sxyzecgz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2oecvefys.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kepmqjbe.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kxktbtfa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qqjpzxol.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hjjskjqa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yctlvrlf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2yznffqxw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xywmmmrf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gbjlitdr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zhzvjpte.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ixfamned.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2htrxyjjw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dlasryta.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zpkzgbea.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ecetfamr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2zdwkpzgf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dnnmjoac.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lupbtcrr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bdnrhudi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2iwngxxqj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zuoqbhyr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zfcdwlpu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2whqajwvw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xngtwhjo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lsmpbiuy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fyayvdkj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mltjgaku.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xerxiyst.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vvqkmrxb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kkigadzo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2gyuenybc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ntcupssp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2oymfciwg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uqhruopi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ywxgvbco.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hkuksskj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lppyqvtb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yymfqoth.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yejimhmu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2otbihjtv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xzvjcilg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hqbswssx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eajevhxp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2dfzdthsf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rjmuxoql.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ouioanto.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ngahndkp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lpwkjefk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gvobxwgr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jnrofokf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zsmgiobe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xgjurcii.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nxzueuzi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2trkjvrcr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2treggmvz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpwdnqsu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rkbrwtzv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jtrmyiea.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ipbnbqxj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgohrujh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gtkmutiw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipquuhto.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zpagblrm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tsvygpxk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tzgcbafm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rznkfyic.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qgaljbjl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qjhjzvsi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vepapron.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2skvvdkow.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bibccqrx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wnyvldap.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ecbhvyfx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rrlqmxuv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nboswday.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2eevbitps.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2upjukwhw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vmrvdtsw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2stduqcgq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2igghwwnn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2psflmtfk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gtztgecw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mvqyyrqe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yzvabqzu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2tmpuhnaq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2einnfnax.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xcirieox.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rcvsdxpk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rfvscbsk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tsonfwty.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oqowifoc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rajrsulk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2miveinya.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dgtcocsl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uvtvhihz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jzuctyws.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zxtckdoo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gjkexsgx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kbcmyjnf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ahbowwvg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ghkkawip.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ojbopjyh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2gwnyifvw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qlyezjkb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kyxbipxz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gqebzymm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2oulgkqrr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tsijluog.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aamlpqhe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cpmpxdlv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2eobwtctu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fxtdonxw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2armpcios.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xxdlwqye.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sndvkmeo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zywcjpwv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jqgalrsa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cdfccied.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2roakxlth.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ryawnefy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2eznkrtnq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fqcaqmun.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tbzdtemj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2brggddca.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yxuaedsx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pntmmmmr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yzcxbiri.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2clruondn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bmqekcqq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2trmyfvts.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jutpksnc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2oqpbbfcl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jipnvszr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lljrrbwe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ufqztehm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qzgafbpq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xykileye.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2upfwlbgf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gbbfahmv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dhafuobe.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ptjphzki.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dndqvdmr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jqqfwevm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nfgqcjyx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ckamujtb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2skpdynnk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kiwcdiws.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2xlarwlti.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2konoepkk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2oeccwgqm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ytzkiwqi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2royvuzrr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2oyshxook.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kzhxnele.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xucgrqej.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sbdujmil.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2djqaojdr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2fslikzue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wondmpvm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rtdlzrli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvlkhrwf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uandydqm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vfcbgrdz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2kvtiaejj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2iwquynew.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2otansvmt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2smuzbuhy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2htvzjaox.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gemfbvyo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dwgofjoo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bsqmvepb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2necxbrlm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ccvdfsor.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vdhdccdu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2seztlovf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bdurzrjj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kzecegqu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qtytolhs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mxlvzbbo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2broizyca.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xrjdvhkf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zjqjcdsl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hxyjxxqn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2afeosdml.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2izvnpdax.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nrcpgywl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2imywmphe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tpnkinqn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2cqqamiqf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hkzbcqff.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2hlnovpcf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2tqlymhyp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zddqpgsp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vjuhqqrq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hfdbvtth.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2htugfnqe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xrduotkx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gwjbkvyn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2shqarrdt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2iewzqkyc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ogiggddn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dksubgot.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wbjahwtd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tnxivvhe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cwiwozpx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zbmdhjun.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ydypietn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qhgrteno.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rvnuzefd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wtlrfdyg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xghebfwg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nkibwrzo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yzqidjue.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gekcfqtz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2peblqvkj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2golkhszo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xqumhebx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gimngwhh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ojxyttsp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ctgogtnn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bkevtqrq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xqeipjtz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2tsuauete.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fhbngamm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2becugknl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2znjuquni.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mmlfkndn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rlnnmiuq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbvurftw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xmiomytk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jzokijpu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2irnnketl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zskfucrf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vorpwneb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xufqyrdk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2grftzjxd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dgdcpuqw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2blqctvrx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pkxlseob.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ciwijyfg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iszvjxxx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vndvnrpn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2veudyfna.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bfacaeee.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ailktiej.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2aergdmyo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xgfhrvrq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xkzemkor.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ocubscbl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2usylxdnl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qihzcerq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gheberag.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jsnrpyrx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ifpfeedb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrmdpymb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nlhizpbe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jzmlazci.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2aqdfdrlh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sanxdgih.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2woojrsns.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ybivwavv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2opvxoutz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2aocungif.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gvmeaoyq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnftcxjc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2sspvfgzp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2flvfrzhx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2njpssepr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2itpbaxkx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gosgiwmr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2talyvlpp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gymkcdkk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vgyhvhuy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uuatputp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kbeeirsx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2jhsstvna.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2orotnztk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rxugyaci.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vkuisxiq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2micsgdam.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rfdzrpis.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gwkymegz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xzxjlotb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jzlyznfb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2oirmfyzg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xdlqqinb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ebzcntmv.html


<!-- 参考信息 -->