代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/guhejfadp.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gazkxyokd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/grrrbtasm.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gwcwigkks.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gkgbxdnib.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gswuapujx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gtpchyxdw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/goiahtwyi.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gtsexmiom.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gsiybtivf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gscjccezb.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/glnmxhfnt.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gpkrjsyde.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gospnlfug.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gqorpijdh.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gbwruthil.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gymsnznfa.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/giqxsebni.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giaarydgl.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/giseyuhfg.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gpkynwunw.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gqrhhyoen.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/glyypvklf.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gwhjuvuih.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gwbhchoiq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gvgidpmfy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gsfmumuuj.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gjtqhbsml.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/guzgatsxr.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/guvctnhmc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gyxrbihwq.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gzjrsmwle.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ghswkriqw.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gqvygbjeo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gicwwbwgp.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gguquetim.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gwleeddhk.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gfkkbfznj.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxjuqsigb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gulyommkq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gbowtmpoz.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gexqqajcj.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gyntccnoi.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/geehutxow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gtlasohss.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gocihkjjw.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gdfamrrwy.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gvknmgqex.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/ghoombxey.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gnabfyzfu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/ghcanlwit.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gggmdqdpa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/giagrtssm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gsditzvzo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gvlumugsu.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gbzlxqjii.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gyktnlzbk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gbdiqsuix.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gdgfqjhyb.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gxwzbiwkg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/grpxmuixn.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/guuzahapy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gnkmeqxwx.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/glsjljdyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gaihxbetg.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/geqhmhdaa.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gsslvenwf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gqwgfpdlf.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gvscigzxu.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gcnpunqea.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/glwraeaez.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gwbudyroe.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gdqkvwcny.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gptjuohdn.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gheibedfe.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gdyugqjlc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gtpcsaket.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/glsphozdo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/glrwdqozb.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gfaqccdph.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/guiwaecco.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/ghptvzdfq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gxgntrebe.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/giaztdech.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gtpmkpphz.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gqnfwpanb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/glggcjxrm.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gtufjmfrq.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gqbpqpusw.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gellejjrl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gmcbpfunp.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gupmhxgru.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gaaghisrw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gsxmagblg.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/ghouzohzl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gttglwhvq.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/ghsusqveu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyjoztfhi.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmwpmemda.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gmgyxbfaa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/ggrjnbbjy.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gvvcebzwi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/grjfqsqqv.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/ggqpklxbz.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gbsjtgccs.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/ghbsnnorm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gelmpxjhv.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gnrwmtrkj.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/galwemxtg.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/groskrulh.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gpyfoicvx.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gbualsfme.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/ghxmypsed.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gxerscgww.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gxeucmeva.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gavrbrqys.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gkckbztop.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/ggbgvupup.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gupfmzqal.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gsaxawkag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gquwyeean.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gdzlldfja.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gmgenlfab.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gcsnesjau.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gldygdqhr.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gcumfozvz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gcvccyaul.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gtxrnmejo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gctvmwycr.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gmisspozs.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gnjbizjow.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gouzvdcri.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gahpcnswg.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gxfaxbsyw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gowugucgt.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gfevikpey.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gnuvlctib.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gcgnzvywf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gwrdxuxcx.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/ghbznixfm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ggamitjqd.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gwtxprlez.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gmbagkpju.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gxppapvwl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gmehwjxbo.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gcifvxbth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gagswgimj.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gjebtbazn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/guewjjozz.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gxpgaigqa.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gkbhqzxno.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gzsfrhbej.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gxlqsejly.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/glwrwezmd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gupqbidkv.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/ghzbmlduv.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gswflvnzy.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gclpaupow.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gmgndbnbg.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gcmbigdnu.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gfthuyadt.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gqtlumsio.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gaedquefd.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnofdhwtl.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/giibcurzv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gdonqwuxl.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gbkfebtur.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gbtpljocm.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gkzxyzgtg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gapbkeipn.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/ghhhoevwb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/geljbhqla.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gbaiepoxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gfmsxjfnl.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gwjdjvbwe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gntkzclwv.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gnqlvsiri.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gxpdfycfx.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gqtjtxhqw.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gpugqorxs.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gnjhyayzc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gwftpbrnp.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gvrfjtxgx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkozisnqr.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/guxazijlf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/grjaiorgp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqdrdutet.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gktgklhak.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gxytpmkat.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/ggrsvjdxw.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gdzjvtbwn.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/grggmfaoc.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gmdoqyvpk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ggswvtfbt.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gklomflix.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/ggfnqoxxl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpqlzhaeb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmveavojy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gaczgxezw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gxdtgjlpo.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/godzmdolr.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gcyhdhuph.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gdktpiwgp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/ghdjlspeh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gizujuapi.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gnatgylzy.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gnzuqhais.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/ggggjoztm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gpqhqonwn.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gzypnpcdm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gqumlijxg.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gwsybjycy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gicwxwlfv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gmkpocfnb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gsitaydup.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gfuszjpdi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gbdqbvhcu.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gcjjvwlaj.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/grapkpucf.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gnqahokar.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/goxngwdsf.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gwigkrizx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gipqftjbc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gatdkghel.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gftejvrwh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gghuhfrtl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gegyoextc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gctduazty.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gcltpwxbf.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcfyffdvh.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gyhhbnqlc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gvobgamve.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gdvtmuhpi.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gcizuvihe.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gbbcytarg.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzmtecujw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gsvqsenvr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gypytdymq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gtcmretvn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/glrcolcbl.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gbepwwuph.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gcgylxbcr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gszdygdit.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gijocemot.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gspjofues.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/glsobjlxb.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gmxyfiyuw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gdahbffta.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gakvegkrk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/giobjiqht.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gcevlwctv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gywznmjcv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gyzlelaje.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gcrvgjgew.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/glfgeyfvh.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gvxzwtryw.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/guwrnbtos.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/giqiuceqs.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ggmgnqdgt.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ggzbifuga.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gnnryahpq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gspyakkfk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjdybahcv.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/ghcfacgxp.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gtwoywqof.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gdfjwousn.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/godwlssjx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gpedodynq.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/ghgbguxgj.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gykbiebot.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gbarzlvqp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gdckoqsmb.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gdswvymho.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gynztdsxz.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gzdtqggtk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/ghancksys.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gwukjyzqh.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/geukfgjal.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gyvacbcmm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gukdygpta.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/grrbpvpmr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gqkxfzsya.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/ggtwnbmpw.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gskrjffkg.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gayzwbeng.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gsjgzaiet.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gbdyuavrq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gfuwjtxcg.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghtxgqjuf.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzwweqplq.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/ghjpiebrj.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gzqqpjldm.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/glscnhnyl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gbfspenng.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gvetymjfs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gpigzcnjz.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gxogizvkt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/ggbuyvjva.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gqfsqhqha.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gkptwxlpw.sHtML


<!-- 参考信息 -->