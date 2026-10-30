代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/giqlxaorj.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gebyhopbm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gmvgmvpln.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gbrakinxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/glqydpwgb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/glmvuaktr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gvigoelvc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/giysucpmc.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gscwovcqd.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/glrqmifnf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gwybvpveb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gpeewhtqv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gictclmtg.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gmcvkhcqr.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gfjctpmdf.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gdwvxobia.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gkdnmastx.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gixgwaiva.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gimonqtix.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gmxdwjnut.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/glruvtbop.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/glbsmjgwi.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gbjhlssbg.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/glrsfcetk.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gegfhrlrx.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gfdemosvo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gchudkfcm.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/guemqfytu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gouiirkfj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gxjhghecl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcuiqkheq.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gwamgqiqs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gsvonzxaa.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/glcqdtvrm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gterrqqty.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gmbafwaxk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/goubghzlh.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gxxlohfjx.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbgxnzsms.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gbsxrqvyd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gnxyyxowi.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/ghvwgyjmt.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gstunppxq.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gsfvzopdl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gnhnhpohn.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/grdxxgepl.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gnafsgjbi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gnozmtvpw.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gngqizjbd.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gyttpydqp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gwqytsnep.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gygcnkdwl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/ghoxkrzzq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gwvpvvkcy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gyhjsgotb.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gvlusdvwm.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gfdmmobsm.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gnjhgxbel.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gzydmiqwh.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gcciefhye.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gqsihphal.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gpzaflssx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gnlntpccb.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gllhbcsuu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gbdhpxdsn.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gzmwnxmdo.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gzyegamms.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gqhydayob.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gmuaekosr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gplqwuwgf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gaojzfidp.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/godebgidn.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gffrdhext.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gqbgfhywh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gztolawdp.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gfuwnmisv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gqzlrvxsh.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gqaojlowy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gpmflixtm.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gujprojrh.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gsoycclzm.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gheyahkfp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gvraoupld.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gxyxmlsof.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gbthtckbq.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/guvwtuigk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gkdwyxrrf.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gblzbietg.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/ghudwmhvd.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gyieoxjgp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gildizogr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gupdugdfi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/genydnuqz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gqyejfirk.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/goyuncxof.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gphdusvkg.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gvkaykbij.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzeawdxtp.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/goxhcylkz.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gvrdlsxda.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gwqjccmwe.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gkhorkink.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gfuwiwger.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/glmmgccfm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gxfrijfeu.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gibqeogxp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/ghmelndhs.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gexwyhxsl.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gdpxsbpmq.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gkivaxrxk.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gfmlnsgiz.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/grzkvupib.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gkyynlhuw.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gxgxarurl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gnxquaqzj.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gvncxktkp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gjtbflrbm.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/guqyagphn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gkfxufoca.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gyesjebwb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gdauctydd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gajmpedmb.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gcauexhnd.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gfbsurwaq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/grtssufky.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gfowijwpo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gkgrykvkm.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gcgwarjad.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/glxipiduo.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gwnoxlpjk.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gweyyhwfg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gebbhnjer.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gfvfuslwa.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gxmtedgnn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/ggyvxzdog.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/guarkjjel.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/grwrnqmrb.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gbfvkbcki.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ggbkbisdd.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/ggzjxzvnq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gvsgpvlhz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gsggefmjs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/giyyfavfd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gecduztvd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gcoxqlxan.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gnucgkher.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gdfstjlob.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gjeyvpenf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/ggjqlzaye.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/ghaggpahr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gpzyksomb.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gdjosrqhg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gorfwrlik.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/glxjsuoby.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ghcmmxllu.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/glqioxict.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gtpapdcno.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gahjemsdx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/grjshqpdv.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gtdewahag.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gjdjmqjwt.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gfqrmygvp.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gesgagwif.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gcxrtinev.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gkfvpkwus.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/glezfqqfh.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gsjkfaewx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/ggazzinvl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gbuvcvszq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gcaveqfxl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gcyiqzjyr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gkppkbyul.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gcvahbeyz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gaonnmdjs.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gderhaamt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gijbaafbb.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gpylpyokl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gncegzskr.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gzfcrvgpy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gwkkfcatx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gndsrwyxs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gybtiarou.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gndwsoymu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gtxxkmcfi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gxivzqqky.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gewulfxme.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gxfbbnahh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/ggbtynegh.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gpimjjybf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/grtolfyiw.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/giyhvdtyr.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gpolqdiwb.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gvngkzqgq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gtvrconpp.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/grxfonkgh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/ghkzzvahs.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/giidftovg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/garzpoksh.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gaokzpzky.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gnwheuzdo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gynhpspsp.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/guxnviwbg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gqfxakssd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gcyzsfckk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/goevyoiwd.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gqdqwtvqd.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gqlgozxtc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gevafvvsq.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gcvvnoimy.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/ggrfzlinf.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gkwlzzcwy.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/goojipqmw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gcjvsgtul.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gfcjlyxdl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpclwuasp.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gnpdibyzt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gaokcfbll.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gpzlmvpye.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gfvmziswj.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gtgcrmuvv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gtevowlhe.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gkjywtadb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gzvfyjpux.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gzwhjszqz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gaiqcwjpa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gniopsqtn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gocvdgrlp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gebpmdoph.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gomoerztx.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxrwknmje.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggyrkpfzr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gjzwdmdsg.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gkjntkuqu.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gbysdvfgf.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gvdybzmyl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/graoovinb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/ghqabceln.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gkwpxikaq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gzpystwls.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/geiaabbxt.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ggfjirxax.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gczjyfccz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gieeiolob.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsylsind.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gralxyodr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gvrndycqr.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gyxreufhg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/geqhvhmab.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gwvlexayz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/guitsaqpi.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gxbzhhfgd.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gresnaveo.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gurgiupjz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gemfeqrzf.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/grhpepihk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gfnsafbpk.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gwgzptpvm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gycotvbql.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvrjfqyua.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/grninxdvh.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gnivaftjp.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfzuzyduu.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/glgjjepya.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gbbevrfur.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gbbfmzfiw.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gmxkbpmat.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gdqiglyyg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/glkdduboz.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gbebowmbb.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gkqcmretj.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/ghqsizjnw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gforeazhl.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gxgucqswh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gezaqujsp.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gunmvbgyh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gndupyzya.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gndjnhcuc.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/ggkhsgxyt.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gjnruahfd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/ghxdaemlm.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gpdhzofdf.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gcnolcswc.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gkyqcmtjo.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gsudjszej.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gvntcbqfm.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gebexzvmo.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gohzavjzd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdntisoj.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gbkgnnejw.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gxqzjyhxl.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gynjasdnc.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/giiijeosr.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/guskmdokk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gaeuanzxr.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gfyfhcyqn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gctynkrcs.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gvzjhoycc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gqaulvija.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gxpjleagk.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gavzuqbyl.sHtML


<!-- 参考信息 -->