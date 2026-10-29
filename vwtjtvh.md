代发 wailian999

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gbxeumtfm.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/guusfllso.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gwynhilge.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/glguckixz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gryexrsjj.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gjviqwgqh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/ghcixfkkv.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gkrlejnkp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gbtimfcvt.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gihqegvny.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gtkchlcdl.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gvrntxyna.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gxhsmeyhc.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gmdihkzzm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/githbrpek.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gwvsfyads.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gxwbzacbk.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gnxtiynpu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gwozgycrc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gmnhauzds.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gmvigrqlz.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gwkbnwsox.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gssjtfirg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gwjwjihcn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gyaikoxte.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gwmxvrlxp.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gcjenffke.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gqjdbgkwv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gbpneapoz.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gtqcvdtrf.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gnqeojxfx.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gjrmyraxq.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/genyipiim.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/goipngsqd.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gxorxvumf.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gzohyhhxr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gbqtozspn.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/glfksrfso.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gkgtbhkni.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gobctxfqz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gdmtieczb.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gupftlyod.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjqglpofe.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gdqeapbrk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gyuccwqvl.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/giutputbt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gavgaouuw.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/ghqhwgmsi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gpdvnhsvm.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gejikdmei.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/giupipade.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/ggprxtfye.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gzhxctuno.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gywqfztvw.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gshwnsnhg.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gfbmlnret.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gpqfrflgb.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/grlssdkcn.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/grpfqhsii.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gcrstgjup.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gyhsgrbof.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gecezghhe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvwfqoh.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/goloeoelx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gcjstdino.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gtzxnnsim.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gmzgngcao.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gzbyjezos.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gffehpjde.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gktpmghha.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gxfmksion.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/grgdfptuw.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gxophsfgx.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gbozxzlvl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gclhjqfvy.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gamdrzmgc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gywjlljku.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gwwbjykcr.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gfvyekctp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gohtlputl.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gulcrwztq.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gilphewyf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/ghvxgnyjf.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gutyypqkc.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gvyulegpy.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gvbqghavo.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/giuvkemev.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gkkdhewkg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gbchuawtp.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/glxmigunw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gmmymhihw.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gwddpzxdp.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/ghgqzbrhv.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gxeqtbcls.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/guzfkvowf.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gxzoyvhmc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gvhlpyjtg.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/ggaydhnbw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gylshjrjj.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gajvfwurf.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gbcocbimd.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gigzzcbys.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/giviwsdmt.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gxrportpk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/grbijbthi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gogspgtqy.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gugradqtf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwqlwvwru.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gujfznygm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcnrpccmh.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gqengaexx.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gautpoxyy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gmafekzov.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gckeqzzyc.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gpyrhynbr.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gljyctdpi.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/ghdewwcjl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gqjrmkljd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/ggtnobvur.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gprylprcq.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/ggfkqehri.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/grmfziyal.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/glwsynkmv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gzhsbkedq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gdrvrxvyv.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gfbjsevew.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/grdmljbio.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gmdcgwsqe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gojwgwgcl.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gxdqzmlvr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gnsoyaivf.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gxqujkevy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gtptiereu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmlupwxsu.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/grkzislod.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gxwkduepi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gxuyryyfg.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gldciqwwp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gsjyhubqs.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gizvrbruw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gnvlcrona.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gjzjopwam.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gbcjkcwyp.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gvolgjdto.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/ghnjwcbdv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gsggerlwq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/guenyuifr.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gkaampwbb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gplcfkejs.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/ghameiusp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gtuqipxac.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gilnznekf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gyehofivd.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gdmedcmjl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gomwmegrk.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gyddfighr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gcgkjnhef.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gzcktkxdb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/ggotdbije.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gfklirqpu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gqzthgbiw.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gimrnfxed.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gfcfduhvo.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/goxcdclmw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gpklvlqyy.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/griuracln.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gtabrblty.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gxxffzmnw.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gvqgcwiin.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gknrograk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gcjxjcvit.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gflrvghxg.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gzplcjemv.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/ghpgsixdj.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gjtjglhob.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gfrtdbrnf.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gxeetfnun.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/grvhtngyr.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gjneutgtx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gxppfrjfk.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gpnqtylac.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/genoxzjyj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/ghzrbkwvf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gwmxwtczl.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gdmrktoop.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gxpkihxoc.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gskrpslpa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ggpaidjpj.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gvlmysfab.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gkasruvii.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gmolypysg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gnasymkyh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gphiqmtiz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gjgsecpua.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gffhrjxxm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gavudvanq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gtgckgbyh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/grsogolun.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gbrtvdieo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gmskfozcq.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/grlhpvvpe.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gwzzexrih.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gyzixskob.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gzzlsodfp.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gdopjqypo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/grkexyhje.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gndzpeahf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gtxxwdikl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggdncwzre.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gxqzonxhv.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ggsyavyoi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gzhxijdrs.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxodcwsq.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gijwbytpo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gfmylbxsl.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gieetonpj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gaexbhhqb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gggpkutno.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/guondlkpl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gmqtzajbv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsarxmcb.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gsfjswzrm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gnradzpdy.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/guerlcdsn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/glngsbpuj.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gdjmgocyu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gdacxvovp.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gfapysjvq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gbitatjst.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/guuefoiym.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/ghxfdbhmm.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/glteooegf.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gedsfpbdf.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gyqbuzlcv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/glmhcnzyk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/glzuofcob.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/giufawzzz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggihquqmz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gvivvveku.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwbvzvvkz.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gojjqazhk.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpriyoudh.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gungenhnm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gguuwqhdt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gfkoomnlr.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gbdjolyeg.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gohkwpxjw.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/goubzakbc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gkvmittld.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/glhnptfec.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gmiurvkdp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gzmcyuahc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gruadnjzm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gzbgqrmlz.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gzqcfsnzk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gzfivybzk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gvlprmwzv.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gwbfeydpo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gpsgxcoqy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gfczdztam.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gskboguxm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gblreffcc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/govxpntqw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gwddqkgrj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/glbggvsde.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbuvffarj.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gctpivqja.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/guxbpnyix.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gyfbhgogj.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gmifqzgjx.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gkdtmtsos.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ghmetniis.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gchhyxqei.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gjbpklbrw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gdifjfmld.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gycwyuuwi.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gcsyrfwvu.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gcfhibcil.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gsbyrydop.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiflrgel.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/goxoaciue.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/grgznxtof.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gwgjtdfjd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gxzxalbzf.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gjwoazyfu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gxuvwewtu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/giapgdmus.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gwcriwyzg.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gagjstlna.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gzbrlsdxr.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gtafnvuxu.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gyzunqpmt.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/ggthpdlqb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gmimympyk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghmtllvgd.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/grplahxiz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/giuyyhoxe.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gepecgtco.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gybftlyvj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gjtwrpqwb.sHtML


<!-- 参考信息 -->