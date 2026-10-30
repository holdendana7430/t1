代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/glekxnmep.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/glcpplrlk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxgmqvpm.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqojrdqe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gelmjeodb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkelopgxo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gyomaegkf.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/glwjogmsj.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrgtvgvc.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/geidjguax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gzxluvpij.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqkmanht.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gprzagpov.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gfanrnxbm.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdtmlggx.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrpmafaq.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmwynhbd.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnsipper.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gneukkpgr.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gznvemern.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfabjtjm.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmapzinmz.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gihxnytdt.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/grjnwrias.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/grysqgcxo.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gmpfqcdwl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsbdhsfw.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/geeibebrh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfjrycqcx.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gneeipfcl.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geqmqrdam.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnfmkben.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotkdcpmm.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvbcgvngy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grglcnxfv.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhnbzfoh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjcvxjgc.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gfhykstwk.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexhahzmk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgqfttdi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gqznjojim.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmsctkzg.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiydxnmf.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gvikhwakv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpucivbva.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmuwdrlub.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgcqvvrh.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxgizjfr.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gzptwafue.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxadygjrj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gsmjakwjp.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/grifolhtq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsqpqodh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ghehgzyfk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaswdbik.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gyxlfsdso.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gzmrbfmwu.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmwcvveb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzablpqxi.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffxvtxlv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkqoxoqu.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gcnrbkqjn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwkgnezy.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvkzsmdx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gexrqdaaq.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsfqflkk.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjeuyeuj.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkicoksz.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfatpghqb.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gehrlesum.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbobhwbra.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gawqiuvxg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gmxksqcky.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlgarvcd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmyamxjc.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhsjqpas.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvylicwc.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gkkfpprku.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/glpyutwbv.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaqtbpat.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgqbxdu.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcfpvrfi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsqplgmv.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyqekyxt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqwyyfic.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gazfvpdpf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqvphwjp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemmvfhpo.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/ggkjydsnu.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gcyytmdci.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdfkbran.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdskdmha.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gclqxgaud.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gumywcugd.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnnxyuna.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ganjvgwyy.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfymubxy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwrbzwulv.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvgddljz.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpseddwj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gobbqprrc.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybcoizbv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gszzhgxrv.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gobiqlzju.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpqwojvo.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaqvchyg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/guvefhwhq.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfimrblwc.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydjwkzjg.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gopiaaedb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwumxcor.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gcwvvbplf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhtruia.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchqksqlo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdydveill.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqmmjyvs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfytaltm.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/giqifujer.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagtbaosg.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfyjiyzp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gnbhoaxxo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gcyllaaxq.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyrwdrnj.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbjtfya.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqttlntul.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzycxosgx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gipymatrs.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gkxqwpxjw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gstgllhac.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gexxokldu.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdhcphdj.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gkogrkzue.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaksggeb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjolteis.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gpgfdzqbw.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcbehnpvn.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gbbeltndv.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghtjsirrw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebjdvccw.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwesjtmjk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxfmidpz.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbmdutyy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gisitwllg.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/guipgrrdg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfmbroia.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzszdmtsu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gvrobfvro.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzhndshn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gihjidcaw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxyrtfmp.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgdajyox.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gunbpmhdx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpelnzryo.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/glilxvmzs.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/giaxwkodz.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjkiubzoh.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/glmapxybz.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcbakshfu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gvvuzwqhv.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gcfqqdoaz.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkgpfoyo.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gvydndvdt.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszytqujl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerbwopxq.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwgjigib.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzdrnach.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjusrhznw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhtraxng.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwipkqhaw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gubqstqkm.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/ggchfdvoy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdriiovbo.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcrwltha.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcosvhdl.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gpolrxdkv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gheboztsm.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/ghacxfcrw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gslzsqmdq.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxcesuiqm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gzaqkypzz.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gspufhnao.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwetvqcz.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnymbshqa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gougwgaqu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkryfxazb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gyuyrolqe.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glasadnfj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gkqifvepo.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gmethwxlo.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpezithqj.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxaiimdu.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/guutybpln.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gholzkcsa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvwdduvxr.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrrljibx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbersolwc.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gllfoowme.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gopqerxfi.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztpiivhm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsytoedrt.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gixjhxtea.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpqpamxyl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gledcvkuu.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjfjcsvtw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/ginjoxuel.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsitippp.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/goakpwnto.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqmqrlhq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gemcoreqj.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gtmrilfqz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gijqlqldf.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gluwymmal.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqrhcqxi.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynyytnlw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gxagjjjrz.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnnxgzzo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gehuxbbgu.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gyauepxxa.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqzhjvhf.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqffwevq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosxfznzn.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzobnjzm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gborkzudw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeygfhey.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gwwveuhcs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtszzgmmt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukqyqmol.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtfgmavv.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/guqyqcpsd.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmzqfqtp.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjuhaahc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gabjhfmhw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmprkqgl.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gebpwbqrt.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/guxvcping.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/geuuejgqv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkivmbcin.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjguqrqeq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcupurjr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbgjodew.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvubjusx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndadbeja.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxlqtjvu.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/grtskbpcu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvcfcmtep.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnxddgqb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwgwutiz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gwtrubdwa.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjfoaybr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gnlhiftrp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gfhpkbklx.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grataugdl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrnnwsek.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girsznqcs.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpftpwue.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbynqzcf.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyhdpobf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gdhkdrlyu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdntjzhy.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqtduzkts.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjzdqvml.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqkywtlws.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gliwtbejx.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gkbrbotfj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvkpuxco.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrnaftmz.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gbvvasgto.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gyssjesdi.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grjekkctl.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqdtvaxl.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvcvtiyo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvbdvzku.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbuaxwcfd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/ghswzygxr.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/goscmucmy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzvvxxpa.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gszapcndv.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjagytcha.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gueomfkqt.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrzoxpnu.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvhkrluag.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwzqvvajm.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gownbfvil.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galyslijt.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhpzvhbc.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtepsshwu.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/grakvxfuv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnvbhitu.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gurlznqpw.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grwizrxii.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvvcvwrxs.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbbdevga.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwisjdyxi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmzxfsxo.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gbteianhk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkkhlhif.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gekbduiuc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsejjupa.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gudfdxlup.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggudstlyo.sHtML


<!-- 参考信息 -->