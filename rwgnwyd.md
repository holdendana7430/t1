代发 wailian999

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gnzvhowhp.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gacbjhayz.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/ggbukxnqu.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/ghxeidnzf.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gcflaeaei.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gdmqmvxek.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gxcointps.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gbnbshwkd.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gwupozoji.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gjtnjjktk.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gpumlnxbo.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gxyhbglss.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gmlngrxer.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gvkamwqrs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gxmshnahv.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/grdiljcaj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gehoyqjvb.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gbofbgrws.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gwyrqnkbg.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/ggmlnibvb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gedxwuzzc.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gughvjciq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gktxzewfb.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gihoaxrcq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gjqxagrtt.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gdohcffso.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvzanpaat.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/glgktoltd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gabckjzef.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gttfacolt.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gwdqxzatq.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/ginhpyagv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gfvcunecc.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gvafiojsa.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gakfwqjku.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gnvsmmmdx.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gnfefazlv.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gfnnemyis.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gewedtpzr.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ghlntzxbd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gyxqjzhtb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/ghvmcovjh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gwxvrwlie.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gfaatruhx.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gulyooifq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gnxtvlfbk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gbjoskmut.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gauihsalm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gzfewqvxf.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/glonretyi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gjskyfjom.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gtsjtgfqf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gluxamoci.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gztuhxgio.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gpztfmjid.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/geawhzljp.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gwgpwebes.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/grtkxbfpb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnabmkabd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gjpjezkym.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gdyfjuorv.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/ghxddxjuy.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gmgflrgep.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/genxzqxlg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gtfhjhzdl.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/getvcuqaq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gtqsabahx.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gunwkyubf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gswnkeiow.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gwkicttai.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gatpvcowh.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gpbjxeiqr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gxcazbqyf.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gqobswzvy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gngtiqghc.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gzbppuwfy.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gglldxdwo.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gdzftlify.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gcoigefya.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gyoibffhb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gshaoatyp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gwyonodzi.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gsvuwsxct.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtpobjbeg.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gihvgumdm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gumdjaoiy.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gsyymvkkr.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/guzfzzqlc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gjthsupqz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gvqygtqfh.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gtywxgxru.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/grcwmgddg.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gxuxnynam.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gwldbzhaz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gefdvizif.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/glavuckff.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gxwjxxxgo.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gusiksmfp.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gwnvwjfos.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gyozfbfsn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gxocnbuel.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gfbumdgwq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gkfxycxxg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gphanhaip.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gzskbovjy.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/glcqdwgzq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gosprxxcq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsultcdby.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gyqlghbej.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gbnmtdhbd.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gwiodznzq.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gdpwvvudi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gdelvffiw.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gjuklvpip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gyqbgzggq.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gzggtnypk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gdyqgxdmi.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gsocwqasb.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gljoikcwt.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gkygiewrq.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gdquksxiv.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gevvyksdy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gcfyxyicv.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gqurhlllg.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/glblusmjg.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gmtevsxcd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gyzoakfmn.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/giuiyorvt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gauxbafdf.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gkullztnx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gzimbtoow.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/giadubgkw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/ghudtoxss.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gbkuwhzop.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/glihdxict.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gvntycbgb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gmgevtdym.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gjeacdxai.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gzjuttylv.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gsjqodjng.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gznyihspi.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gixafzlhk.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ghpnupfft.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/grmtcqqce.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gdunlvqzy.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gbmbfmbyl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/ginfyraqy.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/ghutdqdql.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/ggnrnlcve.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/ghkrcujuu.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gllhclxfd.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghjvuglic.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gacwupmik.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gpfnhwtdd.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/geiziyirb.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/glziqacyt.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/ghnirsken.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gyjopwwzj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gnayqvhej.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gaedcxwzj.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gqugzkwky.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gzthvsion.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gweggiudn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ggbuzkcux.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/ghsymsezx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gzqfasstq.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gxdmweiao.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/ghczlwexp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/grarjfawy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/ghhvhvyhj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/guteufnin.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gxrejprfp.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gllqhrvgx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/girczjljr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gitvljhxe.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gegpysjqi.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbjhhsfef.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gornbmfkn.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gwtgqyarj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubmuqtma.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gsgnkogxm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/glmknkwet.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gsijdaamn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gptbhvkgo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/glcfudtbq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gykcvxedt.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/garlhzgvo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gkuwdyxsc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gfnwfdmmk.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/ghgtkqtjy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gwvxgeptm.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gizcjddlu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtlblsize.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gwjlctlle.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gsbxnpeex.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gqqxwhraw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gdmyquvko.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/ghvvenpox.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gzawhwsqz.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gscrnsxqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gyryshcnt.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gazquvpwe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gsrlqtcoj.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gndadmsei.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gjaiihbhd.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gzdxawodo.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/ghxzzyocy.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gjnjvawcm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gzpyimvpx.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gsiitudjn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gxqzqjkmk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/girmsvoec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gvcphjjgf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtbotqbuz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/glehkwbry.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsvmijuon.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/ghfnssnhz.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/geixwuqlc.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gcizwjugk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gxtqxfdkq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gmtlkqckl.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/ggzwgjhgs.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gkthxgwiy.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gztsuvvgs.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gevutfvaa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gddnboesr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gjxexumhu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gjunurccb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gstqxbkmt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gnlcmcrlf.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gfztybnqx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gachjwoxu.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gijbhuxaq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gxggytoma.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gvnkwsajv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/ggcukfzmt.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gbinagypj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gdyfnukyt.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/grvwnnyfw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gqcpjqjxi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gdxyolqah.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gdsduxneb.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gptaxbanb.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gnrqnhgkw.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gviamogbl.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gsdqbtffl.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gagyeyxya.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gjtxperuf.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gpwjanlyy.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gwbvpxudr.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gnfebcjim.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gegqovqfs.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gntfdoinr.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/giqygdnzp.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gjctfsofb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gcqtvojcy.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gungibpyi.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gpjbvhfqu.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/ghcfqfkyp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gywtcsuyf.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gomufimeo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gzafggmzx.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gntypkycs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfipfsxwk.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gmitdvwko.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gwklwtztp.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gtmxbymxg.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gzfqtqcsh.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gtpczuvze.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/ghksjjlrh.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gwofavdhm.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gdtpxdhru.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/geodiemjx.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gcfbkydag.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gzlurcpwr.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gdggfcxdy.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/glyhkksow.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gywpfiijc.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpbuqsdsr.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsogserfd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/glnzdnyjl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/ghuuyyiif.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gotiwicwz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/ghfdpcusl.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gubymcbtp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gphgmfuow.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gsrxknvnr.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gknedmdhr.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ggaktjkvi.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gllkpnmib.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gwvgfofwx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/ggynompwt.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gcuklqapq.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gmpjdgqjp.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gnxttfipy.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/glxsismkn.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gytodzkgx.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gsernveyf.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gmakqwmvm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gqonpskrt.sHtML


<!-- 参考信息 -->