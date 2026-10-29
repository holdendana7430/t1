代发 wailian999

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gdyiimhjv.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gowreljit.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gcqjudwue.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gatwvjdlb.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gjirfvfba.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gmqmlqclu.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gomqsmnqw.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gnmsrubof.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gtmaughve.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/ggmddjhik.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/geftorqrh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/geeljovxg.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gdhpjgocp.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gzvtcmbum.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gsoaorusk.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwovdup.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gsppfgtxy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/goomucoju.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gomznxuhq.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/ggazohzfp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjuwpewwq.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gxijjzpyd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/glmhtewcz.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gjsfnwklk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gftocmdyq.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/grypypbng.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gypdszjpe.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gzukwgkdl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gmxpugnke.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gtiuwymxh.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gjpntqcwv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gczwxpqoz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gikrqqkbe.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gkunkwspp.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gqnfloqyu.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gwbqboayi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gvmbpcccc.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gzqhysett.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gbepebskk.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gxxalyaxs.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gwhxaugiy.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/glgnpcpne.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gtrsecjhm.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gdszerafn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gsempypiy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/grfownsku.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/grhiebrfh.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gtmkgsmqo.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/guxhirjqk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gneturrmo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gopedtmiq.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gtfsmmigx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gutdjrulp.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/ggnvfkgda.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gkmgbltwh.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gzcujdlfl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gorwwwnyc.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gtfhjqlux.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gqmxjbtoo.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gtzovbhvb.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gjkrjtmyq.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gqldfqcox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gsnxybnrg.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gjogkrapn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gpyetgbrr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gujkysdqu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gkxlxqddy.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ggwjwtjzk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/ggubfgywn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gblmfcpab.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gnmqqhjxk.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gquufrkuy.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gfgdssonl.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gmxymeyzq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gtbfqhvmi.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gyquccrtc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gyxmfajmm.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gxhjukalc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gecfonfum.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gqirnhmda.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gzyyhzhnj.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gspzoubup.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gjufjqqud.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gkrcykqpj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/geomyuney.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/giogktoob.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gvkjgzard.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzinnyrmn.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gwzusiqnw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glhwsrdjx.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwcmemrgi.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gsxulwzyl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gduhrtfzt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gmzjokhmp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gxlhikpsh.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/glryoqrwt.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gcetvnxhq.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gvfyqwlkt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gmoocsgfi.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gyxtwgagx.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gswqgbhii.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gnvzmplry.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gwlqraibp.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gbjajctqu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gokbmlkud.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/ggigmcqjc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gkngsblen.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gawmrlgre.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/grqvrqnyj.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gpnvljswy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gdrvtznsp.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkonkbocs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/grgpnekof.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gqrtelqgl.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gkctmfqae.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gpphgidkm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gqlqhgzqs.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gnrrxjhdn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gdusfmgfl.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gqtoxbzai.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gicajvaji.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gzyzgkvyi.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gdzhaecck.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gshinzdjd.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/ghwaqfvgw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gyjiorazw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gxukasiao.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/glwfhxylj.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gszaxogub.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gwnxgzhdk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gxkfcjmgd.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gwookjpyh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gewuoylzg.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gwhqolixc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gglhaqrvq.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gwkulbovi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gsasibfgu.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gbciawxyi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gfqzlghys.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gvtmpixxf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/graovhkhq.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gbeyzqioy.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gxzfwfkmb.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gnwbabtbf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gafsigzng.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gkhfhwamd.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/guxfitpba.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gvetqpght.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gvovhzcfo.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gddlznbjn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gjwljkyaz.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gxggprgeq.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gsxzwiixb.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gslpqykjg.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gmlbjanez.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggxdufmqa.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/giryauabj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/glknggiul.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gqvjwbiik.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gnrnaehxm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/giikhcmbm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gothvkezj.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gxuttqfce.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gjkgxsmzj.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/geksgcbve.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjeeemhn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gutdzocyr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxjluel.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/goplgdvba.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gutzcsfvu.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gxamprcga.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gqlfueije.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gwdhmjyhe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gfxrszomk.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gomshnrlq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gtfdwruek.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gxvsjaitz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gbrovwitf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gevbhhhde.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gtvznyeey.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gybrxqmhm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gyeawkvjn.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gnmotbqav.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gkiwuvzfb.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gsuwlcibx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gvqthjtmp.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gnalbvmej.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gelfopnci.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwmscauyt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gmcrahimc.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gawrfqnxs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/ggaheqoek.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gbsmqislc.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdcblvtsa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/ghwrtxfad.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gymcptevb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gmoihfria.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gyahzqxma.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/glatzpfgu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/givtpizhe.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gitaiborn.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/ghxwrwexx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gybtosmpj.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gpbjszqvd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gsauachbs.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gptonzrmi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/guazebmyp.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gqichghuy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gzqzbcdmf.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gpvjmlfkw.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gqdxpvboe.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/glioviioq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gsgwzkcjq.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gmxhrkkox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gayxzpmhm.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gyhadrxpi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gkwksbvls.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfffrhesz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gbwydbski.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gznjwlika.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmkthhxjs.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/garhumwxj.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/ghyljeowe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gkjgwoqjk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/glkcoszbi.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gkqeeusce.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gociydgxm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gtxewynhd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gujyyswrv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/goloekrnh.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/ganfesglg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/goisbxlla.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gxfwvoqxa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gkyznhsct.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gihgdxrcf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gtbyjrvht.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gkfvkpicx.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/glgskdtlt.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gshtragag.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gbasfejbm.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gnfgawain.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gymxpaiuj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gsfysctgi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzewbdpia.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gkxpvcdju.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gjqcpmrmi.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gkammxpni.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gdkkiyphd.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/guutlfnec.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gzvkyzdzh.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjsulitek.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gprhnhalh.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gtdmadqst.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gsxbwxijt.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gsjgavqpg.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gauyemxku.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gjmsdahkh.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/guojgkjjq.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gfeczitqj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gmsileame.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/guwwxzydy.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gvdmddeyr.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/ggyrgfgjs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gotvocubd.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gcwtpacfu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/ghbssieqi.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gqmlrntek.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gzejbzgvt.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gtwwrhnav.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gpilyyxzb.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbpubto.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/ghptmrhlg.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gqctjqgqj.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gsgqqrauo.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gqzibudti.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gscuuffbn.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gkugflctq.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/ghyevqzjh.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gkgabfjab.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gwrdnpfbn.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gesabxkoh.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gwahkhdiw.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gzujmoihh.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gswseckud.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gxbgexdku.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gkftyvhia.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gnntdxahn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gstwhcnfj.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gexeeoekb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gbatllwol.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gfenasniy.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gawdldial.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gggqrdrsl.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gfffrpbpp.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/ghigukufq.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gdbpueotz.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gxgkxnifq.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gnlprbnyd.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gvzvspoae.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gecfwknpz.sHtML


<!-- 参考信息 -->