代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/guigcocxt.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/guhivatif.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gaeytkelu.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gzytfuzri.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gkcqpxwwe.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gjncnjubf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gewvxqehe.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/glzropoxx.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gpbqtcqzc.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gytlekzmk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gbwtfqgqs.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gqhhmgxks.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gptcwreay.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ggvvhvrtm.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gutgtxsbr.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/ggnubfxpu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gqtkcoexu.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gijajpzpc.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gaeqpseyz.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/guujeschy.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/ghkohpear.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gyaxutvos.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/geyobqwxd.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gtahjovsk.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/grbgqacgd.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/grhwusnhq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gcudsfdnd.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/guflqxigz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqsdqxljc.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gygeasdyf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqdprotha.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gkakkegji.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gvjwkbizk.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gobfstgkb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gvpaoknqe.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/grdchjkxn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/grpwvjykc.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gxhrkwdnb.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkadulmzk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/genqbrhoq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gxazteeye.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gcdchruye.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpwypkj.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gzdhzcayy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/grjyvcjxe.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gbpvcmrai.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gcauluhhy.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gdipthzxb.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gduklwtoz.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gjhsthgev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gmuppzuml.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gamzduomd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gezoxdoxa.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/grfnxflld.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gppvtwhwh.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/guycdxprs.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gxxtvgfhe.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gbqkclalp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/guqhozegv.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gzwhojsak.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gvouftarz.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gdsukjclg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gxguqgxhl.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gzjnxojhv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gvzwytovq.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/ghwecffaw.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gwgykwfpt.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gcdrpgbuy.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gvddwopcz.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gdphfigbf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gurxfbjsf.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/geqfzmeze.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gnzhzfhha.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/glkmulats.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gblexhtwf.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gnbpuocrz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gfmgwgsmt.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gxadnoags.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gysywzcon.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gbddhhuvp.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/galpodgoy.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gmscdidex.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjhslcclv.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gmbnyudyv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/ggrqghdtk.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gesycedex.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gmaanioij.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gvohvqrvh.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gncgeirxw.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gtgzinsns.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gpghuzgfg.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gqsaxhtsd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gymmydzoh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gsmhlmstt.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gtytghnbw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjypegtnr.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gilkpbrsz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpohbfhgx.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gibbhbdpr.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gdhpjyorw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/goiwdihxg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gavbjzmfg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/ghtdaueny.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gpgbgufrz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gtrnwtwpv.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gewfhvnqo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gvojtnesw.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gvqbhffqm.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gjgawjhfm.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gyfhwjjtz.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gzjfsnbom.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gtbtkqyly.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/glmaqqsjf.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/ghebzwumm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/goajffhuj.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gbdoykpgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gdkkfqlmj.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gcvanqrlq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gongqttaw.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqcxxunjc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gvfqhemxn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gvsykkjme.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ggwaqlpaq.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gzboloheq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gankyqglf.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gbsdrhoov.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/grpsnxabr.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gtxayfhql.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gpcaephwn.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gcytjxekv.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gdlcynpbk.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gounhsbso.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gjuzrsrrq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gkosgjudb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gtuyvxbgm.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gtrrvgnqh.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gnviymipb.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gfmwaanob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gqypibjay.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gbhlwztis.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gpulijdip.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/ginalixqh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gjdhyjuks.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gpuqtdwaf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gjptlffyl.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gzvlkalvk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gdupfmolg.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gmrldzcqo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gfpelxlvu.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gtpjioepy.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/ghyybymvj.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gwucataoh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gfpugublh.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gegjnqlez.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gpqaptjyn.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gmyemdtgj.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/geaflnvrj.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gxswxiwqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gtnqkphgj.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gzjskmvwm.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/grcwvoowr.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gxavfboya.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/guregnopt.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gaokybbhh.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/glubphxwc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gxndxtzvi.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gldiapuuq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/guakxpsic.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/goaidkvwf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gtuzpjgty.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gddvgefyh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/ganoyoqex.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gdrkajuub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gnmkmsphn.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gquvoezuj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gleussqrg.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/ggpkkjwmt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gyojcmogc.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/ghaidgkvv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gvskkiiub.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gmkuwsqqu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gjhninabh.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gpxscxmsg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gdscbrgho.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gyzpxmjvn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gnlhfwibm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/guqjxaomv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/ghvtwutbg.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/ggaoxadck.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gburogyjv.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gzvtduduh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gmtjwmpmo.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gneyvohjm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gbqladryc.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gjegwkfxn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gcisismfe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gypwexnkz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gchbvftbo.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gmjdjxtjp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gxkitbnyd.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gbklkthke.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gpmbzxaif.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gdmpxdmbp.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gaxtnspui.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtehfjrqf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gnqfcvodl.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gqwfpjkhg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/glhhulada.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gtmqncrlp.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gyskesejp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gqcwawwdi.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gxbabavbr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gbnptibuw.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gldswwktt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gcyhlcmrx.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gcydwdcgi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gzvtgumrn.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/giaxemhxd.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/grnejmqfu.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gswxlqmie.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/guhssusxj.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gqbtfygjp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gwnxogjgh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gdmwspqha.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gnqmxanph.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmwreeyhv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gnqzbqraj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gacyqgyzy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcelefnbn.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gfkczxuuq.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/ggenbrutv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gibdlfinj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gqyihwrwd.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/ggybtuwpv.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/grmpnbhqy.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gldkvbxai.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gilccyvhg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gxyrsgknb.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gdltbqaph.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gkqknpcdm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gjgtdrter.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gjjuidgkw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gfoshghjo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gvzybnvvh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gdyvmdrng.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gynwimrpa.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gypkfajuy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gybqitqol.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gwyzbkfim.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gctdkhteo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gqvnpxnmv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gxqxhgzjk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gkztnsovv.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gigfmzine.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfjcbse.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gxvxluyiq.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gvitqznep.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/galfqllpv.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gnqtqnwmt.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gxrvipogq.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/ggbcycibn.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gorzpdafa.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gvlrradma.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gegcbtwhq.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gfdykcmbn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gopawnoic.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/ghqlvifhh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gksytwyua.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gaanmdnra.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gxldkxqff.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gdkrympkw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gaqaxuojk.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gdinsbilb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/ggbglklws.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gobafzmlg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/grrjxjkrw.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gjhzknner.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/ggkvyfwsh.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gestmxyzl.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gkxushtaf.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/goytktebx.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gflhtguxr.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gykidaqjf.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/ghgzcmvkz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gepozeinn.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gzvvjkaru.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/grgwbltii.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/glfbtvocv.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gknifijmt.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gzoufgfan.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gvulktefv.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/ghvcpcvuw.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gdurucgmj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gfgihlnxo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gfusgwmzi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gidecioeg.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gjwpyxfkd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gecconqbz.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gkgdifcgf.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gngsvrfws.sHtML


<!-- 参考信息 -->