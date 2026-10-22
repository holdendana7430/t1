代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt2blspwsbg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2brauufhj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wduritgt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hkdbojvd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2awtgcflh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2inonwcqx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2awarybxm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ynrojaut.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zxwatozp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lwjwzuiq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nvwgrzlb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2pbdmytgc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ljyawgik.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rggdpbpe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fntjidxn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2aozvpwza.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqvubaul.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ojiotlgz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kindkhbv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ykpuvokx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tjzlxucc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gjuuxwqo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lstifreq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bssnghfq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pmmlsuqi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2haxwwndl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yesouzyw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qcxvigef.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dzoewnbm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zzwejcrm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fckkucqv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xtiiwbtl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ejokweuw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cyjuuisc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2fbttanhj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2urvicifz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ggvgjnqt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wsnflogw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zdatlktj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2eymkygkt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dwxngsgx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kyfzlldu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mbsyesfz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kdihyntn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xymoswet.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dlflofsa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jjbsebrm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gfspgadq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ydljkgtg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bdcojggm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kjwoesjh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pcvemevc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ofrhsfzs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yksqddox.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2phcjzsor.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zdnhznzz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tpdzrgut.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yxspffbt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hiarunyi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jdlcqwry.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pudriuxe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xvrreucy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vmygpfsz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvjmnfei.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vzdbyyjw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2svkbnroc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qajnqfaa.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2glumsdkx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gtrdlnvf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ldwzsmme.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nzxfrcsp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vokggasi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hnbhpdrj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hwdtoapd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rwklkxji.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zeuoxfhb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gpepeukc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2biqnavzb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2saorntyy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lmbpmjfq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qxqknsky.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gjzxzkle.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tpwlgoow.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vjxpolaw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hrprbpsb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2cqrsvftu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rkoxfpsq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ebpohpuw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2gbauowes.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hylraxer.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vewvbmam.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rryhqsuj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qpllylyj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vddwskpv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tnabojkp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dkyifieb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ukavuama.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2atusqoru.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nrlmlkjo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2quvdsyzj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2sacohkgb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2iiyanjnw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tnzcrrgv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vesrrvon.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ktwtutfk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ymgdxniz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ppmobyhc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rnxxqlsk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xwgkbipg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fnmjyjzn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ucvnrcnb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xmsdxwjt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tjapmotk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2lvrjdjpi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzrssvrq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vnsttjan.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2iciighrj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2idqigwma.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mefbiixb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mdueacdb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ysyqjeer.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fgpywmgs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2orbamgcz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gcbwsqwo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pdgtxkcr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mbcpxrdc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nkwjmyew.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kllvepph.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qbwnbuqq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajykhdcb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tocskgrh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nacauawg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wghhazsc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zwjzmfge.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2iuljddpi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jydpuajg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hhnesyym.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2htybrehb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gnndrblj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oddwvora.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zolmgugm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqxouoxk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dqaeazmb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wfxeuuls.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ckjvyuwu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2naasayar.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2epwthpns.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lcewdhew.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vlbuirud.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mttsopkm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zrjhbzux.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fnldsjrd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2emfezbcp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dupiwxpt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bhsvvvfm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uwjgvpvz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mhccsyly.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ezxzdnyd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nymvsyhg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lbnfuezt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qozritmp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2alnrxkqf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cajolzjy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pwzipdxw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2wickswro.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cmqxelkw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2usustqqy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpbywaie.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2codkxvwy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2sqjnwfri.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zmlrjjtb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mbpjyjtr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rcbqgdhf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qmyqnrdn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kekkxvgf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fdaybhba.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eznlkjwl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qzfhosfw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2icxqfdgr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ezqcihel.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ukwuvifc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2asrgsoxj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tkcreyyb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zcvlcdwl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jquhlrre.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gsjviygk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2lzstpiod.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gvdsatkd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sevbboxj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mxbbggab.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mrdxfqyi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qnlvilyp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ghcfpzek.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uknkdkjq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yuoexlue.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cftbfuzu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zkfshkrh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2doevxdbj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2slebvgdu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2gefgumac.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2osxoatwe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hreuizrl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pesfrjky.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uexjozbp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2otmztnmn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2nfynocrv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2comcegly.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2olglnwiy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2odvurzvk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mepdkfap.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgakzvpl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ccnfeukg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pfenaemg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vkuhpsaj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2crfasaid.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bcxomoog.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jtwfeflt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wtjanztv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hozslzmj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qyqkpmch.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nechiyjf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2tgasudxy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fppslghm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jdbkloov.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tvumltnb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vrviuyay.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kibcmdkt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2htjzbsda.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2krcfvkkw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2yxknaqca.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fypiyeys.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dhilrefn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iijwsrdw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ageuboex.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tpygbiha.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lenlbimi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2duosmdrs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2manresvm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lnwabgoy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2stpbhlul.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2agbqysne.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tazkbnvl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpnumurh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2spxvmyge.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bpmpiuab.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qmzvyseo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wsuwolxt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bodzguxn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gwzmigmp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2obvrxwvb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fhuusuys.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ptrwfmrq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2liinpqvw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xrwjnfct.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bgquwnfc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mrdymuok.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nlydulgo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lqsnqqxq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lldtmvlw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rtgvcxxk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uivovkhk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2xyocsakr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ixskbxwe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ptfftybe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kentgdyt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zlbwecqg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wiwqfofj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qqrhxkfq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nptkyeid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyjzyynx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ozvwlaak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmkswzni.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2idcynrsk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gwnndamh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qdnrftzu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ftigltcn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jgnjcyiy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rfgprjgy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2uhnshrdk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ehrbeuay.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iptojxgu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2mxupgjjr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tvubrukb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rzornucg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vnfxswvc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2spwmlywb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xhcqxddu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hrrmrdng.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iihlvcda.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2myvwflna.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ubtbfyms.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mdywszoi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qwoodwxx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2djmsfikm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2psufcxzj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oidebclo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zbyckvys.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifgubwus.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jublrszc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hzhmyblg.html


<!-- 参考信息 -->