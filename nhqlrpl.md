代发 wailian999

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmupmmgjc.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gwwgufzgx.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqatfiqjj.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkwiigsl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwudcichj.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gwytveijg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwiigrbd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gggvlfcmj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsjasnqlh.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gglgtrubo.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/goqrvghjc.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gelrodrir.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/glzivkevv.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmktissl.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyykxkdn.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/giiqqvhkg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/giquwnbip.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/guopwamtz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggilpibbx.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfcpyybd.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gykivdyut.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gnweditay.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gutufejuf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqabxtmda.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyizufvx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpnfubcx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxydfljxh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwbgepaj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gwaffycft.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxuczagd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/govreczow.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuppssuo.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyalzngpt.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gavwzepxf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gaobqepfn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfewihwcn.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwrueuen.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gaouppssd.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gshosexmw.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/geemceadl.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gioelcscu.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gczyhhhfq.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpfqnwbts.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbrgoghi.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/goukisixs.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggozjhdsu.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcfctgut.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gycxdcmoe.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gpbvvouzt.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gyrjsarrm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpplztcfp.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/guxenuwcp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjasxfnsl.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvujvukp.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnywmzbef.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkifyuouf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gvmqyysfh.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxigpmhic.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gymqgovgs.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gurwtjxii.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gjnanacss.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/glqiivtdz.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gymjbipzb.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsvyzbin.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/giujslmqt.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gobvprjen.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwldrbohb.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/greaoomff.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/geitvlkfg.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gsldpinbe.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gzmegpedj.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gelrokuxf.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gsodmvnju.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahsudzka.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gulruvuul.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gysnpsfpy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/ghmfxrbku.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfobubeha.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghblylvnq.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxmvsdqb.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gmtrxetiq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbisjbhiu.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ghcsmlfdj.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaizmgoo.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gilpghjcr.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtawlupcz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/glrsfdtkd.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gqmmpgkpk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gywdomumn.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbxautvc.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxecnwwuy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/givzashma.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtmwbxib.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gkyhdpmwq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggjptxtkh.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkbrfwwy.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/grkzyfzwv.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gywzesuer.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gcavkppqh.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchjuanxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gfyrllcur.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gdprdvfsa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gabzcxssx.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfnpsgmx.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gvlkzfejr.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpkhxjxp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grstlayhw.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gttzuqbhp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvkassws.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/guoovjmbb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnxihnry.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvgjmscz.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ghorbsqls.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gmuslaesd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfdsmjbeq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlvzfkqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclcseice.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gqhpveodn.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyokewbr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gohdiwwzq.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqgfeedug.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwqwkmtp.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gldetkzzj.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gdwgeprfk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxidettow.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gpgkcygzm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gkkdctpsb.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/ggmjtzrhr.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gtjezhhlz.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gfytnjjyt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvefefxp.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/giewwxvyz.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwaoyzfb.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdduzwpk.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdtfcren.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/giipixuvu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigpnqeym.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gdfpcygex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxkmxgfb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ggancpbsb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjedvsij.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhbrvrxc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdpmxkkd.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbvdljgu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gazidpaim.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gvobfgwlr.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfhfvmha.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/galasgeii.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gobdpzuxa.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpnduuup.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gdcqzpojr.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdbsuhho.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gedbzqipt.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqahdudov.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggypqgoxr.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/ggorvoxks.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfoufncf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/grcgurygg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgqretpe.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsotstlvr.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gnxaeocef.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxxgwymn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacshmgpo.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmszmzzur.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvrctyoz.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gidzfgieg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvjwfyiy.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqherahc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/guxocokeo.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbhtfgzn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtckzwscm.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gfifoihsl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwuhdmfw.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gknyehklq.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gisfwihow.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawafqwhy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbbqebqp.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvjaqcd.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gevvyfnhb.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbsibppn.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpferjzhd.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtlkfugu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gafwiowis.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gagaxrdvp.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwlcudat.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gcuvnettf.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gwcohooqv.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdjqbkrv.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndzwbyif.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzobrqdt.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxklfqwek.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/geicfavau.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/ghacyxksj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmdheebw.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/giyhvpinm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhzcsjsr.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnymxlpun.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gummqbooe.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/geftyafoq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggsvawjbw.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gxupykwcl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/githfdlqd.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gccslujjt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnmwcyfr.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvxrlivyk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gadlnbsni.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbhapjcpe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxmwlsxl.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gydtrixdt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/giqounbrd.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjlrbuqc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggziuximq.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdpbolsd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gbhxcqlhw.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gbdqmyncz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/goxuqrnag.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/ganjzjljb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcypxsmom.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkrindtk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpggqsoc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gkptlxkzp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkovsnyb.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gulovppxl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysonhtof.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/givsquszy.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gamyqfigi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgybkwxs.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/glpuqriea.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gyaycjtuu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcbaftdt.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gogevjtdc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gdclygzkg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gelgabvfm.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gzjdmarod.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrmnfnxi.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvsxxuux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/goqtlpcxh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngqwzggg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjgxqusn.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gbluckfgg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvureifq.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdgalupv.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgtcevvn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcgamtcu.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/giryykroi.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvawzzerd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfwiuylq.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glkckbvpq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrzngaiu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyswqckbl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gatlvjhnu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gudbyunyp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcttlsuon.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbbdvwtpx.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbumuvetq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/geubzxsgj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwzkrbvk.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwzfmrhw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbgveuxz.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/grfyrzkyq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gtleupppo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gtlsjgpld.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gyasuxrja.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvgnmuye.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gntsdpgoq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/guquwarsa.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyexqmeft.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gvywfvnem.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfrltyndr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqyyzhyk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhtpwmvi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gxoaxqbnq.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gutqnrvcd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gernyarls.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrjkgksv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkukczvel.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmqtghmr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grjhnwuvk.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmpdjlks.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjgtmhx.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gacrggoxi.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkjslgyd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqqequxi.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdvjqtdk.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gkesgxpmu.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gjejdtrzo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gytwwhhsa.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggprqfwcp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnqsffou.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyizoqkb.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkifycbu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gitoikvcw.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/grigyjzvt.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkhjwion.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gajwmoazb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxzgpzbf.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gytanskbh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvtcvztd.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gxzwfowsj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfaabndd.sHtML


<!-- 参考信息 -->