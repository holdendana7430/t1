代发 wailian999

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfzoqwqvf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeqprpdw.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gygtpqdcu.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnscwwkn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gevlmuhia.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gxfrswfal.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdmyzmzm.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtwelawel.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrwkemkr.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gryxzceiy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhigwsuh.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwzbyncdl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/goneqmkos.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzpqzwle.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrdbkwad.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gblvcrnzj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gmytrboyb.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtxamojw.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjuybzxmw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gsxuwlnpu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gecxvokmb.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjveykwxb.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkytutbyf.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gxwhfaecg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpjflrwy.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gapxaghkl.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzpqbqnf.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamhycwbe.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gxahspdwn.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfndrtvhr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmqyzdvd.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/geqdiqwqr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqwdkdcq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfczwoko.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gnttwsnnl.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gxshxbbog.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/grosklkfa.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/goidgndvf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gdbjkinmn.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoiojfyj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokqoines.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/glyokrsbl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkensazzg.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gtcomedmg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzszgsmt.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gccaxcout.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlztsjpa.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gyxltidhx.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/glnqulyfx.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhhtadrp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvozdggzn.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/ghqpoftzl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgszydlq.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/geixlqlfh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/guoakrwse.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gppqlhntx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzpeoexs.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbizlgiv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdmtxdoj.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ggqbnybhu.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gwijzfivc.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnovqkwf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmpekqdi.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/grppzpmpc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gnegvwlxu.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggytpdatb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gzpovfsip.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gylvanora.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gymegfjsp.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gkgexlkcy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvrsrtemn.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gvdbzrenk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gienuqprq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gwcmfrigd.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrbenxyl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxlgjdyda.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxvwmyks.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhijtjmw.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfodbntx.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gouuagpcx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyozpplm.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gzflnexaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzypykrsn.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gaeozcwrc.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gfjviodjk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtbqxaep.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gdxvmfjud.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsthokuh.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gksezscyr.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gamvlkyri.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gznodddkz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gykqtpuyk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrujkujd.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gefpzfbqo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gqbddeokf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/guvgxmqag.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gagporvol.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gtbhqbpsy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzzkbrih.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnijlnkav.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqitelwka.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiubekbn.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/geuwjhcyx.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvenpxsgm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqplznifz.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlmisapw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoaqmdyw.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwwqlspo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeplyrii.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gquctuzsy.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkvnfgfo.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gmkwyzgqu.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksrirybx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gscwehjul.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhwzwftm.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzmamsidu.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/geeestrlq.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvdwvgql.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzwfglpi.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gteznvvej.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjotezji.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gphckxccg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpcnspfv.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfyyqfhd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnmggvpb.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gnhiqnzsb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwloczvmz.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gfuxgtmlz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzzwhwwd.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gsrzsxrov.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmmrnfgs.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdlpqrmz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gexavvzma.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gzkrrsfbq.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpftymxlr.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gaapgofco.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpllvdhw.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiadqjzt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gykrfvops.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/grjlaxwdj.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxohwzanj.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflxmogiu.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvfumfvn.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyqzdqfs.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gitypcown.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzjcdwdf.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/goozmsnue.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqhmncpw.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gatnzvxtx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gjzcspurp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gylxkhhmh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdjvspynh.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/guhfwjggg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxbzzzdpa.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/grkfblhxl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjviwaamj.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcugzzpn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmcjjczv.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjhotwoj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/giegwapfl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfxqqjzsy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmggcjcx.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gimwyjeql.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/guwpuksig.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guwdbjssk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghapcfdse.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdubnjfux.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdmhpoky.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gomwegaei.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbbvhfjt.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/grftnzvuz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjegmufgz.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvcojsxv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gxitsyzob.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gbhrauvah.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyciwgaam.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gekgikfbv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxznzbap.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwvljsbj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gsyzvtcmf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/goajcunuq.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhurfaqx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbdujrks.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeminhvh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbroawvsj.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gcmgfozcv.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gabwsawoz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsxczvpo.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaxppezy.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gqreohseh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gzcexregj.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhlhtfcw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggztnqfvt.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gjuqvhewc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ghnjhscem.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gpeipjteu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geuhmozbr.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiyptbay.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgbdjwcu.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyepxdhx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmwstxkg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwaqqdsz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gerukmkli.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gntkqnnbr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/glizkuprw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghddoybar.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmxkybbb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnsuzocgv.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvphvhejr.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdatyaygo.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnivduxhk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeplcevz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gewvfnhnx.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gjckoklja.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsteunhag.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gixmbvizx.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gayazwpyj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghygaaisl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfbbylbsw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoinjbcq.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/ghypmxrzv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsseggnro.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjxtrztg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gswzpckas.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkygxnlom.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/grmjtirnf.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkgrpbavs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiigggqb.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlakshah.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gftmfzoyz.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gdmcguuru.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcqisubp.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/guyojfpkg.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/giaucjktr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqazcync.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuoicdhc.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzyejdty.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkphahoce.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbsftnab.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/geqwzqghp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gusoyzvkv.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoqfdmjy.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtmddzbci.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxegkxuj.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gocgyrfge.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqavildrm.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gozaeahvw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdqjcjme.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfwkmfna.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/godsxgzql.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gyymymziz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzuiqsyf.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaabisjp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gipzmtcmy.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/grlisihmb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gtkptvrbx.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulymxpgz.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtmbxcvd.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeoriqbs.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gzbcvzjgd.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gugdbremt.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdqfubax.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gudospksv.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvfzfdxt.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gdrrksgld.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gathhwcrn.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gxljtehry.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gfhtkskms.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzmvtylfz.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcdpttad.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbsdfrjrj.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaeyhkvf.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkdqksxa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsnscxic.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuebegsy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gjpercazh.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gpkywttln.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiwzuueo.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcjotonda.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppagzubo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gngoyfnno.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gwfbmndwc.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzbobietq.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gyztypfjx.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjqxiivpk.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gipaalasl.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gcoypvneb.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gozyenqpm.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjhnhgxzq.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgwynmeq.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkndjbgka.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtojnrbsx.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gogvawfup.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdgeibxe.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gotjnwxtu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizueapid.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaijqsyk.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gktvgswvr.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gyrxhgvur.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqmqfagg.sHtML


<!-- 参考信息 -->