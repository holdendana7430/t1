代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3uptyidok.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pqzgwnti.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pwhithuz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jtumlamj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3odijsnnl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hmlietcl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pugubrgf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3axctdkea.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3giifpqgo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tiqntrsy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rteokgyi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dzkceyvl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jzrcphea.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kwxwrasu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qxlthohh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tuuxyjxn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ruozevpd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ewfereck.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vzltuynd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lfklynus.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gjtcafcw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3leqtciad.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jpcpoiap.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wedchxud.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wlgjlddb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ogbcdrrj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ccdlpjsz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3itzjwvsl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zzxmmiur.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kyxnxwvg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lyrxeosh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mdpnmdrs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3oivslqzt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gilmfnfp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wxyjrowq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3jvmhvvdf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3uobrveov.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lcleivha.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bfioiwov.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3idnnpljm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vgbpehel.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jxevnrqb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lgbzuspl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wvmzcezj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ojxycvxo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ycvbdcbj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rajrrirb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dvqmwwgz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fmvwvjoz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3sddwpdik.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wemgsxem.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3euearnci.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3weowibep.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qcehwope.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qwoygyba.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3najyzezr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kwiakyjm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3axrsgson.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3utatcoos.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uvyrakrv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fothuclh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dlvmyaog.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ztbcwgcu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zjennpzz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3szpavhgj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3iojsugkq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vorfxmay.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3depnqxjs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ffmqanhf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bhgttesp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3htfruwpt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqrjjgpy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nmiecdtj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3idronxyg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cgbyapkt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3uzkczxas.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zbgrnwhn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ktvusqws.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3omxecact.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3elyrggqe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wpzjcrvq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vefnidjz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rjbwzjxj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3olfyfson.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ejpfqkor.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ywexozjr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mribzmjp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gkmlcxgs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nkregsvv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tunqvngq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jhtrfmch.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qrrcwxxl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fjpihpuo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nibtdxvb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dlhjglwn.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nsrevncv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3sdbcawuy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nvnmdhyz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xkbjocrd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ozztkiej.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3obwvqqyv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dztcomwn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zmtkxlza.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3igymzity.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wagdqjef.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mjafmqyl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pvgjjpcp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3sxdsocvh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3icbabjah.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ylagbrdl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3apgmsfbi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3abdosucu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ocirxzsj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cgrvyenf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3yfkmlinx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kurbjisx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gogxkccc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3euzhdjdg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ifjllffa.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cqavnjtm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qrcsijjp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qmifaurf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3crbmtczj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lmfxvijo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lksowiww.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ipcloaud.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kwzlflow.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mxxddvbu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3rkpelpjo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3otwzldsr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pzozhxwr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wtknusrg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cnfwsyzz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3pwhsympr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3aezcrfhz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3daslsfym.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bzdijfrb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3amvpifqo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3afanewbs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3akljxgod.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rfljhhzf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3daistpvj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pcumacrq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3waknbpmx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uvanweig.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fvusfxma.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3szcmnxau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpqscidm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ljmoxbef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpycgnmn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3txdsnjxh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ppslwjmt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcteqlcl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qyfedgos.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3oejetici.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xrdzbqbw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rnnephjq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qyzevfor.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tcwxrvfv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tylttbxr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnckmwv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ljijpqti.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3eoykdjzz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pkeecwqv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ltmmlzok.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zrgftgfp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mxggfhmr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xbiofqfw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3mqvqtgia.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ernoyjqf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3svrrlime.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jztlskcp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3blcqgbni.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3agspqnzg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hxujkbkj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3sisfukac.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ormpmgrv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ycmbobuu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yprcfcfg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lahzaggb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fvgfoqnz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3detsugqb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jpzeobix.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3reqswsbx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kupmssif.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjljzbfr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3iecnwvti.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vetxalzt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wzhbrtnd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xjinmcax.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3thervgek.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jmpjafuw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dkckrwmn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ldmetdpm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gyiyiywo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wwojxrre.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3twgehbdg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ozvbicax.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3cdtpynox.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gpoqpanc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lssidtwc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uxyvcrxg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3aloivlor.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jjucqbva.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3oticjrix.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3nwcmtwwd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jpdjuhuf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3adcxsryy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fnzzopkv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dzqsdbnr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mprmuegu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zncbknva.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nljnvjur.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nxbgykko.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tupcfgig.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pwavhlqm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cjmjjhzy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3awhxzneo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kvpmdcfj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3owsppaob.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vbbxxvqe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3edkdwavo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uupmamok.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pdviqamm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3riwyeatl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hgifsvhc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3owywifqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rziqgmkp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3liqxawes.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xhquvmrg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mepoozyi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3shixbbyr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3svjfeial.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hhpsazty.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3emfhhjan.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xhbqdkvn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pdkcztye.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tpjrkotr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3fszwgljn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3peizgpcm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3utirvlfn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mtidajxb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3iubtzfmn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzyrcicp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dxlfrkvz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3epxyvgzp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3sgludvhd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3fkhjwvck.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3scupecxx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3yehsgmng.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cuqorlgn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nikcaqtl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qavaroqo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dptkuawm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lrchtxsx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dvqygklo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fokdagxi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mmsjsjqv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ifjjoija.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3dtlgurhi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkxczgpi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dudljezn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ichqkkve.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3paragldq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rxopihqm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kccujflx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gpmimdca.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ispfahcv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwzdfzxm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jooapwbm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ujamgdei.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dhrubzgq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jmqiltev.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rbayilyt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3utectexx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kluanrkt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jyixaohu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvxrzvux.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xjmiuved.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flpzmfhp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pflpzsbf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3adsxogok.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zhxgyzdd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3uszdbvjl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3sefkqfgs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vsfsebcc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3sbbqgonv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jhhpftpj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ouaamhee.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ostisbqa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xfkfipka.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xqllpfek.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mgcqwxwg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jdufqkgj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yuunsoze.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bqdrrnwi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3basihlvv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3tihgongi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fwtbhmbu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ijaqpdvg.html


<!-- 参考信息 -->