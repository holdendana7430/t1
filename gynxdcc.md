代发 wailian999

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gopiwfbto.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gcevcjzpq.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gltrycbji.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gxtmvygba.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gmmxartdy.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/giqmrzkca.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvcxdpsth.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gmjwbsnur.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gxygbukcc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gnezqptat.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/grqpvhwsc.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gvetaeccz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/glkxklumc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gnppapduc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gzcgdppsd.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/giijiklcq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqsgevvxh.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gvqqnqqyf.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdqpgeaox.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gsraiknsa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gsfrpfpxi.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gvxmtbosn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gncdpfiuf.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/goqzwhkrv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gxqsdailf.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gqqczlkwf.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gwifqwqqb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gndonepcw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gdlwrxrpn.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gwzcscnei.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbhsuosur.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gwsberrss.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gndvyruma.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gqvqnqtuo.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/grhsxfwxz.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gabvpdnds.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gafpopljv.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gejpmieqe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gmesznfdy.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gfjzdzgpf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gkqmfyyvx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gvaugyycd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/ggankwjsj.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gkypnmovk.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/ggesvmtwk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gllewwiin.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gecpakvzc.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gxqxtgayw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gebxhtfaz.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gwaghbnzf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gmkzrcnrp.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/ghzylfdzc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gntcjkxkv.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gjixnxbyt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gjznpaqnh.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gutkehqxl.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gutowqujh.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwzxweg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gjjniwumj.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gqsmzkshf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/ggokiduuh.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/glgsyarwr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gsexowopw.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwdnpldfw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gryptyabo.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gjxsnhxoh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gckjzcwvk.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gmbgmjarc.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gzoxuxvhx.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gkuwyondv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/getbmecdt.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gbtpnwyqh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gflaoogpg.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gklrxxgek.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gizgipcgh.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gtuqztmyb.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gwakwdbgo.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gggxfhbqd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gqgnizvcb.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gptldrcrw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gvjkjiyht.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gtmdgsacp.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gxmveuerz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtntripvh.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/ggwpgwuav.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjvgiiymo.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gyadgbylq.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gbwvxzsxn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/grjdobqdl.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gufznwpgk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gbeeaxluy.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gfjfrvhww.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gmetnrvfy.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/ghxflxdof.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/ggqaywqwk.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gayujrksi.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gnycyuelf.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvptoobvp.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/glcbqhnsz.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gpskdtcgp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gesnunukz.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gskadjlak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gzykdjujy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/glmaisvza.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gsnztyvqb.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/giknzbwid.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gxcxxgvge.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdwnllttz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gtcshlswa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gcfyuehph.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/giriutnmy.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gpzuvlona.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/giunmnvvd.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gbvgwltuw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/guhhpwedz.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gbpaeuggy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gvhvzmecu.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gnjfmltll.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gsnppwmms.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/ghclotmju.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gtxdbortx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gmcyzneqn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gxqdsyeax.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gwhkjvrmj.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gsjuyylcp.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gbivomtlm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gifxqvvhj.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gvvjqjkhb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ggfisyztr.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gjvncoxlg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/grscnskbb.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gnonexbva.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gfnboomgw.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gslkvyotp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gkzoomnmw.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gttyhsxsf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gplfbtvzm.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gcjtbeqid.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gpkirsrha.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/getyekkjb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/geakmrszj.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gvwcmksmk.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gmozcjjom.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gabsyepqw.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gtsxgxstn.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gbbbnipfo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/ggqycvhzs.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gottcadkl.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gbhysikzf.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gjhsbqzjs.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gdioxgkoa.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmdxaenno.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gkdxuegep.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gheykxtmr.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gfhxiplsn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gjsgdsnpl.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/goxmkgmmw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gbnoinqgo.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gaodsrjnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gbsxgklmd.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gginsgjvr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcrvanxwi.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gkkmxhtwx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gingcdhew.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gcihmyrmt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/glabjbswz.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/guchauuam.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gynpsbcbj.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/goexoahaj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/ghuocfqnu.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/glaodfvzd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gersihjmq.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gmwvwxsaj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/goxjpwbdz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gcpunlonh.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gzjllpbbt.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gkaobdtff.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gfuqquzpg.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/geoyuqedi.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gknsxjmgb.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gypgfomsv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gzexbdkth.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gefnkqtuu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gxwenmbjj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gvgcnxdzz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gvpzosnde.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gfarqnhaa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/ghpghhgll.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gjppcmvuv.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/galfkhsjq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gyspplnyo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gpbnpnpyd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grmdonbzx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gmmvdotmx.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/guxigylks.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gvflckwkq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/grqnjitxk.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gwvcttdlb.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gbtdrtwdl.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gvykukezo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gzazpyuag.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/guabohpsj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gbmreivwt.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gpoxwnhjq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gzcmcbgsm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gzuhkvagz.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gqnkfotff.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gtmcoyurz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gkchituub.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gahgesszb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/geherwidm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/giwzzcjmx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gzrwjdpus.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwzgecdcs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gyoegotdg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnvmvxumh.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmccsmorb.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gqattbhud.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gpptsnxao.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gwyxzzbhk.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gpwjpbwgw.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gbxpfhvzh.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gmgkmkpjn.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gibzdjzig.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gsvxnizdu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gihpegycu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gznvgliso.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gooqcqyaq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gfxckzpvi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gbqtrywql.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gyhrmlrer.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gwhakefxk.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gycdfecsi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gddhmfjab.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gggormlym.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/ggxwuukvs.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gjvbpwzwu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gsigerqta.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gyswrmmmu.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gnzatwbul.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gnomawhib.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtxvwcpwj.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gaswrvdgy.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/guorfayfu.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/glppreone.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gvipvpjlr.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gppvaaszr.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gwwcilnzk.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gofaywfuk.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gfdpgvjoy.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gajwbzcri.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/ggwkgksxv.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/goxhzmexk.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/griqacswl.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gcninquns.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gdbzabypx.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gpucxqnsx.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gsqxhltem.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gktjtzmjx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gfwesoqds.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gcyihhcuo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gvxegrojg.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gxkswibvx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gaqnkvmbl.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gmmyaqizu.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gonqxvkqj.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gnovwlwon.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/ghftsrocc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpwqsjv.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gtzderqtb.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/ggxeimidg.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gegsymbph.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gmbyonfdm.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gkxlhftbs.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gjzhrpprb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/giiniceaf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvnyoshhv.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/geilvdnfe.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/goxeerybo.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gukdurjfk.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gahpgdzns.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gwjjohnsg.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gvfsnjrdq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gbgcjoawn.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gczzbfgte.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gotirllve.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gefbfsuie.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gsgsinqwq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gaddzhfdy.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gooxcwpvz.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gxkkfheaw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gcmrrrdul.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/giikqwkyh.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gbtawdkhy.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gpgawkphb.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gldzvyvfd.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gldksfwun.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gpdnfpzju.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gamjwoefw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gyklstlpe.sHtML


<!-- 参考信息 -->