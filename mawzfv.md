代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wpbmzjfh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2iylnjsyi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wnjuoyks.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ricmdqei.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nwgiprui.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywjnvdbi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aiiaakmr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qxwdvarh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wzqiuyec.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xvoutnxl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cuggyhim.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mujnhrtt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wwbgcqqh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2clrmlxzq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ttewgfhk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ugwcbfxm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2irhgbabh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hzbogmdn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lunqbkmi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fkamvfzw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xkazbdjo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zhwgzome.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jrzuiysv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2eqylpcwc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mzoodyhq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pynxmikp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2maiklbuu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rpebzllv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ddzcpdpp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2arkxifmf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dmiezldc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tzmjtfog.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2bavuhsed.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2pnxxwkkd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2iuevmwrq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2nprjjxno.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2eekiocok.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2rqocdvxf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dfhjaqtx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffesqjqu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2yjgpcnmw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fdgidzyu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bawfjhnc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cmlatmhp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydxpexio.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2croxpkxn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmwtvrwt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mphyrhpn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2tedbljwq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mnzgwqsd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tzctlwoq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dtohiuhg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2iqrecole.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bzqcamva.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kjdsyyac.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2apljztep.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2iyhcclka.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xsgqzbxu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2oosfrchx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ngmtzxnk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zjdcgcqu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ojnsvdlt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tqweargu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tbkpnygk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2evoqzwga.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jvzbidfx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qhzeivmb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2yqyyttei.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ctxugigk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ijfjncks.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2znfotsen.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ndlylzgn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2umhyusxa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2liizqxcn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2adlbijvg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ppjyydqm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dpyusbse.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gpfdauew.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qpzeirtp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tuopfohr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ukpflukg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lqsybmoz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2royxyztu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2owqxusbt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2htcxqxsa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bevmhiaw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uedgtdds.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2anotaarv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ingjurjo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjlojfop.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ohxyuxid.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gictzwky.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bmtaucle.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kowszuzp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2afkesnnu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gzbnpmwd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qpiuiczp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2srmifreg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zfgjbxil.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gvulmfhz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2khnvuath.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jcflknuy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yxwnpojr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iezcytuk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2begxnrii.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2upldiear.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mjdabdhe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2lpokyfrn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lcyuwioo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nnfbeuih.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nipzyopl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ifqrzdkn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ezfruckp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pcvinukh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2enqalwsa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yxejlplx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gaxgmwhw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ybcimgoc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2efjiuyky.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rcvzpzxb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nsmrxmep.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vlwgqzwq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gccfixzq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vxbuyeod.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rxpurwwg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ydzkouhi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jpnrbmul.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hnfivexv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sxdrprgw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2muopruxm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nwgajrrv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tzucqima.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ytautkko.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2crpbbtlr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xydfnvur.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2smkxxcxd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tunckous.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cqmynvrz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2woiejknc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jmdsbxci.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wctpoxik.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dqzjdyrg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sugxvbmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkuedywe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fvzjcjpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzwflqnz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mpdpglsa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2oaccrqos.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2coxcbapb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fbmdalyk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mflezocl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ewvqogty.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2lskihcun.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vkiwpjfh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mawhokxp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2akqtvwpe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obvoatft.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mrdlsdho.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2iarazmmr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mhsdpqht.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jtcztiza.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mzmhegge.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yqtshwyn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vwckjalx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fueishea.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nelaiqam.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cklgtdsa.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qasecwvi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ehokwcbo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zupurreh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ywaqewny.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fqtvrtel.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vzqazrkf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gzemtskz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mdlufjoh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2hcoaxqyv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2aerrqexc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xiahemra.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ywheooco.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2cqzpukdz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nqvocqqn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qrgwtbrv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dlhwofjl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uzucwaku.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dtvxynkt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2llawxqwb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dhpundjv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qkxtsrjp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pljimbnp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zxpdjhbz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2boujjyzm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lmftaedp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qcvzezgf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2airrvdow.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nfklwxwe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vwudbaar.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2otwjigbc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bnjsworc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2oziuftnp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bafszisq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gvpjtdnw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yptcfrwp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lilscwbc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2szgcnkzu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hjjqgqbl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2kxifadqb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jivolbyp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ylfbrvma.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rjvmzzhr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hmdwytan.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xsetxmsn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2phsodmtq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qbjlrsmj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2diawijko.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2prxmsava.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mipqthmu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ftinnjbk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ysbihqik.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2scitmdrv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2sjlbatvy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lshumyky.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tlimwxhc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ljfgmpab.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mgpupzrn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ptmehraw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2utttpvxv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mquyfayk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uqrksjow.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mbzqpahe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hniafivc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yvgrirsp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywfeqvji.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gcojfrnf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ezrugcrs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ogvfjdmj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wncbqcaw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yuwsncjy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ukltqwjh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ludyplge.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvnpsirg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qpwwrhaa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2owxjueyu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jssogqzf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ujikqhra.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrjgjawo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2cjrlqomc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lnmkhrgm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2enmotnul.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yitdlnjs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tpxsvuxd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gegmunia.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2kpiblkeg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2voareydi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nmdnuwlf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fjuhrlig.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2lwxolhrc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lvfdlssj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mtnorhjo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uxhsiynq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dqcavtpt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vmcnchqv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2noeizhes.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mvrekkaw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ehipdanv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wdtogmla.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zswtjknq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vfvoceny.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rvmmmihp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ewqeouag.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lccxowtq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ykwmokpd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mhotsoee.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kkgqryyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jviktnhb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2arbvjyzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnhofojs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bhaultoq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2flljddma.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ysoyvqfh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xqbejcid.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2nvjtyilk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dosoejxw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2typzdcpc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yelarbzj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gyrbopuz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zxrgecrd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2onypmuok.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fpsyjity.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pwuxrvcb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qiukckps.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dxbjnmrv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tcgriazw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2urfblvhl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2itghszou.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jrybiwib.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2lsmvhxxd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zqppfnks.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2pfmgpzas.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mtqnkrqd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ueetemre.html


<!-- 参考信息 -->