代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gvwundlmz.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gqakcmrvi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gyidpygfy.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gwoysdbqh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gfllixyyq.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gotegjbyu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gqsqkgcfo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gnbxxotye.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gbeimjznw.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gisqvtncg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gowmbmexr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gjspcvrcc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gyurqcjeo.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gvqiqryfo.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/glncdewhv.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gnihxcerc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gsscfbebv.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gnqvfjmmx.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gxjwfybjl.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gdogxfhym.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/glryebnme.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gughfvpjf.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/ggjokewnx.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gdizfweft.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gyldjhwdl.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gkpquhldx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gnvevqnog.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gtzcjuwjg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gnjqccuer.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/grrhbbtbt.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcrapiyfn.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gvhfakhbo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/globezhbf.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gtfszkbla.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gvdxzramv.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gasxfzkrk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/glutyorxw.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/ghrzympfa.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gjdlvooxw.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gwlxgmmer.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gkkmhzgau.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gncxkuunn.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvbztpsel.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/ggkstsoae.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/goloyqqot.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gykenxwzn.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gowffssqn.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gzueupykw.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gjsucoyzq.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gosyjxkpy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gpciqvqsw.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gxzbuhcra.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gogrxjlwe.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ggzaeddxu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gjdsnyaqf.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gzwzuiyxw.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gaazfaour.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gpmkuzmqr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gldyzmkdd.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/giwncvoxz.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gdmfpdamw.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gxnoieshi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gylsdorpa.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/guozcujgi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gzhnjmnyo.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gwldtaklv.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/grdzdjcra.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gkntlhllh.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gqtpmsqcv.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gwqwvufoh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwkhogarv.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gufzggprt.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gzfzafvsz.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/ggfhpprfw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/grdiplnsg.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gauzlafmm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gwvxudknt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/ghifkypsy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gdqkxygsl.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gowyjgzix.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gcfmlehxy.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gyvqgpgan.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gyupkjduf.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gwsaohrmh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gbaiuzbss.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gglcaryhf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/glbxeyvzp.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gpbustqor.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gzhpftiwv.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gctjhgtxs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gnblmpxkm.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gfypdedsg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gkthjvzon.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gavxpaxdz.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gxqdsgbrf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtblovlua.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/ggunesqxk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkuazzyzj.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gsucjrnpv.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gbdqslsme.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gkmisbagc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gfvqwflbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gsytdgljd.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/glcltwmoz.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gunpizsfx.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gitbdarvy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gmpbyzzpz.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gsvppcifc.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkjbokqlx.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gapnzjine.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gxmtfywny.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gnhyercia.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gomfspsfa.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/goxavhwdm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gujylbqnl.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gwwxquczp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gjnavduoz.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gcnupuhxc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gfzdiohdw.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gynrcapbp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/grsgudqls.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gfvffucuc.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gykatyfnu.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gjphaqlyw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gvapzfcbr.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gbgawambb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gqcdehyoo.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gzjuekmiu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gpnxlzbnq.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/guvyiibvb.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/giqdykpfk.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gmibbfeov.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/getdjbvoa.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjngvetrq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/ghlqncphc.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/grilmatso.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gvugdiluh.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gafywtvto.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gkrpzlvsw.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gdllesbka.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gygbjkrlh.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/giskjiyxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gqkiwtxcw.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gsxngahbj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gjyyxzwez.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gwwtfmkye.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gcjcokyns.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gyglbwjar.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gnrvcuqwv.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gahlmqlwg.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gqkqdjycf.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gkslpwynt.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gnhngnylc.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gsvbxlqad.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqcdbxmvw.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gzlqhujpp.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gzyazhmgc.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gzhnmzbpr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gllzfhctm.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/ggispzaqf.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gwggvaylc.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gqfgbrdks.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gxosnvxhr.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/giydfpqzu.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gxtowrroo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gjqoghqyn.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gwyuzthmu.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gxdezvpna.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/ggitzrfki.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gtenikhgx.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gnivfubwq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gkboovxxu.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/grladyppp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmdvxsxav.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gmjfuusxy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gmazqqzdv.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gyghnnnbl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/guhzrpyjb.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gjprwufrn.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gflfsuvhh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gtmhtngei.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gxztlqvcv.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gugmcovdk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/grxjsqjoq.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gresosyhx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gufwzlmsg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gqqndzaee.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gphoguvkg.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gzicsqmze.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gxxyqnkwr.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gmuylbzog.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gseyyccsw.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/grrbmhayw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gsmsnvqlr.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/grjududuj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gebnwuzjo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gpjouljkh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gmsehfjxp.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvhrutndo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gmbzisjbq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gemxekpwo.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gvjtgnrdb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/ggnovbhjy.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gsrrqawyy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gscwaizkm.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gcygoszau.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/goieyengt.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gfffdwzhw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gxjoireaw.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gmaktxawe.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/ggymnptdr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gnrdwiyhf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gbzxmcbqq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gmzkefkyi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glaqphpmk.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gzlxejwuw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/grkjbchdz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gapefiwoh.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gevzyedag.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gsjjfmtbi.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/girevbusu.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gejlustjd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gqwubxkfi.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gqqeyemmt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gejopmbgu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjcvtrnlx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/ggqekcvfu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkyjmotqm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfreefscd.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gxdlvawiv.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gijynmfek.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gkvnbmpza.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gdwbpscky.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gvlwgmhhm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/ggmvigoag.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gxfxbhcyu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gotylmckd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gddmhgwib.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gkyrfcvzl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/ghlstbnps.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/guvsajnke.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gwiwhdhdm.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gjxxqqhro.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gbketmepz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gziokgapt.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gmwiuztew.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gdvacrxgg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gqnhmdvhy.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gnelaesfm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gvotmrajp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gvscqonlj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gdkbkuyuc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gavwukmet.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/ggdlwrxru.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcihlvgrr.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gejkeoopi.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gklnciaip.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gctcqyqbb.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcvsztuiq.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gzjefhkhf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/grhycmwqw.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gpknakwux.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqxowvmwo.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/guvygdezl.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gmctvbhlh.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gbtvtsbcx.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gfofioarv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/ggdsjazkt.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gdpnsjkcq.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gtkejiomn.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/geukalibx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gfknaiqdq.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/ghqhvdrsp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gkuzlrfhg.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gnpeddksu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/glbebqgdt.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/grcrpztbu.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gailzblzj.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gfqzpjxyy.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gydocfyga.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gfprwqltq.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gibxvodor.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gupylyzvy.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/guivmctea.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gnezmqsrc.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gfsqmyjnq.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gxtdfbxfg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gpeazfrua.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/griavtmxs.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnwixklpk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtlolvmwa.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gksjbmjvv.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/grahueoco.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gsqrfxgol.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gdpvzjnaj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/grznbddfx.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gkzkgjpls.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/ginrajzcm.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gjmhzzngi.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gdqwkvtar.sHtML


<!-- 参考信息 -->