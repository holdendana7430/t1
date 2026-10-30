代发 wailian999

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gvujsxfla.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gywtvhrdy.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gfuzmibcr.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gbsipoiwx.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gtwplddqk.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gdtbpwraf.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gedisywjr.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gnpmlkyho.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gpirvmawk.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gypkhjglp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gjtrvzrcw.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gmgcmdiii.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gphetlfkv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gogqvtcin.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/geoanzxaj.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gljonjwtw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gbzikajxk.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gpbbhrrms.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gwfvdnkdp.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/glzagfkuc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gtvuyyhzd.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gehpkqbli.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/godquduxq.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gnzmojdpl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gtayoqpbm.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gsnrjjrab.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gzyvclkts.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gmdlqthec.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gvzzpbdmr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gjwgijner.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gfkfcdwfa.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gvwoksxbi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gkjhyvugg.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gkwotpchk.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ghwoncsqu.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gikyeqery.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gzsyxwjaz.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gcgpqbbaj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gxxphdaha.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/ggrpceeeg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gqngnepdf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gtzilpbup.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gaplshdnz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gadqhqdam.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gisbbnyuy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gmhddawow.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gtpinvesg.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/guibplixa.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gggdlyvil.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/ggdasueaq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gwgznpzyx.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gicmgfxkf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gbwbpjkht.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gtqpogkca.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gffoujzba.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/grvgapuhs.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gfxojcyni.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gbzfyardz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gjonvzjpu.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/grjdjgnwl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghfnwldtr.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gauxpjtfv.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gllxvvlij.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gailmqucf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gfzruumng.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/ghsufdgbj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gykktxweh.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/glcrhaicw.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gddgfdbnl.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/ghyzqszzl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gbtsdfdqr.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/ganrfjefk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gjwgpogju.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gfeufzjnc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gofaliunn.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gurjqdvwc.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gljwigjyi.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gmbguaeze.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gjhsvnumb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gdoumgzzl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gmabudxma.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gtodguhti.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gdfsbklef.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxmbnjtjf.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gxcdcnmpl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gadziwzeo.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gphghtucj.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/geygakszb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gkmjqmsuz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gvimqlceq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gcqyfxslr.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/glghohchg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gccxcgrxt.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gdbznfbpc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gvlythzfn.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/ghxcvqbga.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/guduhtnsb.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gtvlozjbt.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gclnondnn.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/girwnimkb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/giujzqwxl.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gijuopheh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gykupmhyd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gcotvzaga.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/ghgnfjyii.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gskwqddiz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/guqoihsvf.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gzvzitqtg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/ghtwbtzzz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gurewvfqw.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/grmgpsosl.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gihjnyrck.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gnbayzxyi.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gijfqeyuc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gozlcsxhg.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gsuofskqn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gjtvinrtm.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gynktqtle.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gyljkmcwl.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gfhegfkbl.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdlitqori.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gqwyhpdel.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/grsapkzkp.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gnxmpymfc.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gmofzkjlx.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/glmdagyut.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/giskdipaj.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gyspruiti.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnzxvrctw.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gbxinwihi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gbydpubjj.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gdzsirgcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gjowoimdd.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghkzpggjr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gwrpmjvip.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gsukuuffp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gwntztqib.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gucyvnbbq.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gfibyeuef.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gpyylrgul.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gcvljtkau.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gwgquuoxm.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gmropvdsk.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/goszvihxx.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gmraeaugz.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gvroxorps.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gobzpqzzs.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/grbamiynd.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gdlyroqvy.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/grsditley.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gtagflfwb.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzphasnws.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gkjjurctn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/giwufhhgn.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gdklsupho.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gbdatqgin.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/glrqxnvxn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/ghyltsplp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gwogjgtki.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/ganabuovk.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/guarnzrhm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gvqvfjsoc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/geobehyvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gveoabldg.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gdbyhoxnr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gsgstgtwt.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gncafqceu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gwlttzljl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gzakgqtnr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gdyxkmhph.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gvtnqfmlc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/grextuior.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/geiowcyqc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gfvoyaqsx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gbhyvvkiw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gvtsgejmu.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gqnbsbcmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gwngdykbv.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gchebmfbm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/ghraofeuc.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gdosvwqmk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gtwhukfet.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gqtvilvuy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gpkpipvbd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gdiivbfhn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gpstkagzn.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwdmhvqar.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gwejpduzi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gqkeytfgi.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gbbvhjjel.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gzxpickli.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gnvootiwj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ghcfjupju.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gtdbntnlm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gldoxvami.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gjowpawfq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gppvvghoj.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gwjxlomxp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/ghgcqvthn.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/goqvuzsev.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gdcappfzg.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gmmagwhyo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gpckwxjfb.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gsrdyuujt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gguqqkezh.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gpjehwuds.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/giericsqk.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gqpbtgdoi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gqbqwxvnq.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/grwhvcjoo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gmukireiq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/guzlhwqij.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gxlgovbpz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnsebwvnc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gjiuaxset.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glpfacxvp.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gptfcmjdh.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gxcwscuvl.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gwgdgmavb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/glzrsvpnx.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gnjtnoldj.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gopxeravu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gjfkkkizh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gaydmbxkt.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gmyanphek.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gzszjtakv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gyqzbqnke.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjeicqdto.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gbgtgiaob.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gvaznjzpz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gcqywoytx.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gndtcfxms.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gwwnoekde.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gxwpykthi.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gwrgjeoou.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gehcslqwq.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gnyraqcwy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/genckulos.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/giczxrmnb.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gjnidxsmp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gujteksxm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/ghvrlsrhl.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gezhovvjp.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gbbnkjrmq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gvbdfolbm.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gzihaskjr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gaqcjjnfh.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/guahnbciw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gomuvilcj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/glaqifynj.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/ghylypxxx.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gthswyupk.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gzizzbzmu.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gcvjytbcj.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/glpegewhp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/ghwkapato.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gsnfjlnjj.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gzveohpcr.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gnujgouic.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gisypcrnv.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gdogiuzkl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/grqwcgatx.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gtfbagbpa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/ghxmpfgsc.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gvbbwvrpj.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gpyhnrohq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gnwtmoyqh.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/glqztinzm.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/ghjfpnxfz.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gzprqzfzc.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gscalexoo.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/grqyojfms.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gssueozol.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/grufinerq.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gfdoznjvl.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/guivjehiz.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqapfntdc.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gdcfuaitm.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gicwzfkgc.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gijadknkt.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gwihsebaz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gsljyulxj.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gzsqdggkv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/ggydvtxuj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gquvpsgzf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gvuoxawpg.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gikylmbkl.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gmetdjwre.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gnumdcbur.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gsdihpfoh.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/ggwkkhysx.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gyixttaza.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gnnvgemop.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gysynpqhc.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/ghcehujxx.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gyqeurpbq.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmdqotcns.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gavpffpth.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/giwwriilt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gqbnpivsw.sHtML


<!-- 参考信息 -->