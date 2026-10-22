代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt2etjrbhmu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kkkgeipf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ljjggstr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zkwnsfka.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gjfovaem.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2akmswjli.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ifxuhdqe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbstwyzp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2amtsnrxo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fcuidefe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mpxqtbdl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zxwgaxps.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bzoxuqdn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2iauddzgg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ebzfivfp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dvizqfoj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2urfiyodo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2sfzdsfuu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aifnrfsn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2svzuejgp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bswojftw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sthzegxa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yfwcupni.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fataqxpt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rshfralm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2geqmerxi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gzhscgrj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2puluigbe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2swiznuvg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ccpxjkzv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rrixximn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hvlzerat.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fwwcgsob.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2etdmsbwb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2weczvkvr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lixritzj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vuoozhqi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sxikwuzt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2thutudmx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2svkwigmx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwwioxi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2cbwirall.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hgforsvy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2nwoyohnk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dqlqbvbr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2unofxrre.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2srorhiya.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mmvkubom.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lhvxnsmk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wujxxkvz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bmcrpewd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ndbqeahp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fvvoskjg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qundrjsm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2smcjgygo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2sqiiqcsb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lzcgmvus.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pnhkletw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tstuiwgf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2irnweitx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ujtoafci.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xqmlmicf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zahjivtd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2fijctaso.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2iwoloohx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lnjxxwxu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wdniummk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cfbcjblv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bemmzwbv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2unfpdkej.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2sncwwejf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2brycgmpq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bmheupeg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nldjhqye.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uatclvdp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2sxubjjtr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2naejhtks.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qvcjrqci.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kmnmxmux.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bibkscbz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kpkbxdfq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ivlknrjz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cuvpiegu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dbqsfzky.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gnqpucec.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zvvypqje.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sbsfcppb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tfcncxdd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bvlpmfne.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2seouiasj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zronuhpz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zgsrinun.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2eurffmfu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2treqthcv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2epuoqrgz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yortasdd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lsxmupvu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ddepprlz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2uiitulwr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dkcmmspr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kbigeybf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2apeundve.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ipooqkwd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ywcioaip.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mmyvehwr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oqlirqxf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mwwndzdv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tdnnddmi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kqaoplbp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pagropbb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2regkkypn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2utqmidoe.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2awkidppf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hcrqkqah.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pdzmxkvp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ehlqoiwa.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xlcrozjm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zyptwaqa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mxcwvgqi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pzlwnkhc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ftpyunmc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2oaxitwqd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wguthfqx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uwpaplcb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ezftkqrr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vzhptabq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2csjyqgpn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qltkdsco.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lkxilhmv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tdjxefta.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wxssatlh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sabqujrk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xpsqjrqf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rzfnbhyh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hmvwmmwd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nmtclnsw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xzjgrebv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lrcvgqip.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mfupkcee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqmcglfw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gjkwjwic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxionmfr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ofndcxrp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cmqkgvfg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2khnwerza.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cyucycve.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2yaqeafig.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2yuusjags.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vexcjrda.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xtueifoc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tjgkvfqc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bozwiysn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjefhwjj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tagkhcdg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2epcmwnnj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2wwgozqhi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tujsghhq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2exwobwrz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2aqbhaotc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2soieciub.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xsxgdmgd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xtpiuehu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aotjijsp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2crsvrabj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2udwpfzzc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tjsnlwoj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oihydsvi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjfrsrry.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xlmxwgmp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lcvkcnmo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xdbtagtp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2iuvuuysr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wmysmzqc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rclbfkam.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pmglfphk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mpllibpw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2snlzuopq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kwfwqzwz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ihczqlup.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2terowqtm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2elvndxew.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ovzxrmsr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2teimgoqc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ckkdnsma.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ivzmjppb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2iisoeakc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gipptyln.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fkfhrkco.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2olrttbge.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dxsxntek.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kivbuget.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ijybkicf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qrjvjebl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2shnqtuaa.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2aejgsoyc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vtybtmmc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zehzdoll.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jnkiwznc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2npxfjitb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2qgbfkeha.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bmgigmki.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynmoldsq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2eecfmyjt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jxzjcgre.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cuzzqnvy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qsvedsqj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jokcbyfg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ouucowar.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hydxodfr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoezuiwn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ufpmdrlr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2apbzqgwu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gijwhtiy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2legocrxs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2oockmihv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbumouae.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bjmwhphm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gbqbfioz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tdejydha.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dnrancfs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vudmsovj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2onizteuq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2uhxaoauv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mbqvhzkc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gwkogpfp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2phisobxi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nvgetxqz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijqdwuno.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qddoldsf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pwzrhflb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnhvhljz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dsisaync.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fzrykuyl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ukybjzvc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xdmeqjwg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzbbpfdt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2whieromu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fhwmqowx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2riplehhx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mvmkshwl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xmicqetz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdekylws.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2omthorpx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tbpkrdzr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tjqgcvio.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwfzifvm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kofpntmc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zqzupaan.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cuyvcteq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhoemreq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tobtswps.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ijkfkjoz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jbchlzzb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zbpyxkve.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ehwvqkai.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2amycjtlp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ersqovfy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wgtnblca.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2khejrvxv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qdczhbjj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qjwsqguv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hvgnkrai.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2smifhpsj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wvehpmov.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwoxaqh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ytmjypah.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dnaghixv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pelsrpoh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bzmqjulc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2viapkujt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2incababs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmkrazpa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vawzhcxt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bwqoqjjl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qcsolhai.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2cewsazyp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rymddtre.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qvbigmpe.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2numqoqov.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pybeqnrk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qjexaine.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2miuoqtcf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lezxxwbg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jdiatyvf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fhtbqonp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gidribpn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kuwahqhm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vlpqyfzz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kccfhpzr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ibeuycub.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qyexkgrn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2slkxjpfb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gkleaofb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hzhefehs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kjzauzbw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iiequpjw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ykvefpsl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdyxjbsy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2efrifizn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mpcaekfi.html


<!-- 参考信息 -->