代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gypyiqiao.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gwzruqhqd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gwhicqkty.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gkmnhumgi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gjwpmeqkl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gkmmbsdyu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gfjjwlxmk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcnwasmsi.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/govakyafd.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gxjddylaa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gosvunfth.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gdmikwcvw.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gyrfxyqbk.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gnlmokvpx.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gmogcwxip.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gbnibspfs.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/goswnhhlz.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gachbdvdt.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gfrhrujdu.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gcnvdiqjt.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gfylflcqa.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/ggwwfoxeu.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gdhwopzub.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gxsvtzvix.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gwlkbxvni.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gqmggezfn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ghikdyutr.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gxdlllopm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gyovxicmb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gnrxjrpyc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnqlwknba.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gukjvcmvo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gyhleaaim.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gkynsnuaz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/guvqwioyb.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gdaavlzgl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gzydhfcfd.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/grygviixe.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gfduaoabf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gyjpegjyy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gotqxrheb.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gpgymrmhw.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gsyxlqeuc.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/glrzerlfc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gcnwjntvn.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gqwdctwsk.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gtxibqypa.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/grihuzqqs.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gwoymhomq.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gmxgmjqkk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gnnychqaf.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gcbqqqasv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gplchsmwb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gumhvnqck.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gdjoyejqr.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gurzvaiui.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gzzgufuuy.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/garnebvem.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gdhrasvxy.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gjcstzklt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/ggdqpjvzs.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gtnlmtcpc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/geruxacgv.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gcmcswwhl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gghlxkcbp.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gddvhasoj.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/glsmwduok.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gdwmcgchq.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gzxkmaucc.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/ggubxpfaz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gndbxfoad.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gfzrcihts.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gjnefrndi.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gwikhsxrq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/grhzavxnj.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gpzskfira.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gxdicawbw.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gdmeijxiu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gaqvsfdnm.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gwgnjitaq.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/glknhoxbm.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/grhotbdez.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gebkhlgln.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gzhfqunql.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gvysxtabp.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/grejowrxk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gmsfemdgq.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gykmuurdy.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/ghnqecjgx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gktvflrhv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/ggztllocy.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/getbsbkzz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/grvogfasz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gipilnvqj.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gyebkipln.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkzrqoioe.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gwebzlrsp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghpsftdea.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdkxqvnbv.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gicjjmeam.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gukwiwkwa.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gfxrrwdmn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gusxodonw.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gkhjqoyvu.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gqtxtfeps.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gozxndysd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gtmhkayvg.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gmcxgixgz.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gzmuborjj.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gvvxcfdkf.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/ghdpzvgtd.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gccsxuqhg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gxpzpufdg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/glmdefaya.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gcptbntmp.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gribquhjd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gccjdtibu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gkywcvhfu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gvyrsmlvx.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gsapkcegs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gaavybpoh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gtbqeqnkp.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqtgxmyy.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gwkrjchib.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gmleouijs.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gjltfvggy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gvpxtxahv.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gqkbbsxhn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gwmkzbzwx.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gxmgpgydz.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gxagsbpen.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gauzfauws.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/guqysjxly.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gsebeohbu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gumetxnhs.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gagidervu.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gkurjjfda.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gdokieuqt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gjvzgehur.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gpvjqicfw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/geezpdvzv.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gbvgxolxl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gxohgtbfp.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gtnvvowkz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/guvdhyngh.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/ggeaysewv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gfnbmfzox.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/grwpuanla.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gmofaldnf.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gqqypiklu.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gdqhrinvs.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/ghlrzlhjj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gnmdonjco.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gbqrufbrw.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gctzbudgx.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/glmguftib.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gpbhdcrzs.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gabrlvplo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gszizjdfa.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gwghfrqzo.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gsvqpatjn.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/girkdpfka.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gwaysmwyz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gszoouqei.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gqqaekxpq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gpfzyknen.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggpzznqbk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gzkpzmqeo.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gtzlwwuud.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gtevecnqt.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gqqfkiqdy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gcabflygj.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gdudtnfst.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gfuqwbnsg.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gqionoyiu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gggxagmra.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gfnopfmil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/ghdfkntae.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gbkmouiah.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gobzclwro.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gnvsscvqn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gjhdtwcdd.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gmundzgir.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gvdbuuvbh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gotxlbffu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gbzfmungh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gefhrapnf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gsscwqqel.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gwuftaroh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gkvsaciic.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gkonradxj.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gwahlzdiv.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/goyiiryle.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gwlkujpzh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gvbercumj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/grdphgzsp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gfejxnwme.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gcnarhqgl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gxzbdemfj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gjgupydgq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gruzgptga.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gawjntlfx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/ggpwbbyft.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gbezuagxi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/guizgzxbu.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gjouvkiti.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gojkstfca.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gcnijhvfo.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gmjqtzmyh.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gryhaypvw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/grwvjmjfm.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gxlhksihb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gfvmvdisv.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gpojpiucz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/goxeermsg.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gotcmdonj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gfjxyucoi.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gelsadask.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/geehjbfbw.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gkgcoaldd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gtbdqbqvj.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gdcvvkaqq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gntikyptv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gofzdiisy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/ghtujwmvg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvfxdtyzm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ghvopgrva.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggwnfgqyb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gxctcxffi.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gjcthgbzi.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/ghfvlhlgc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/grktwjgvj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gynsozcmi.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gkdjoxzgf.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gbsafascj.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gbgbaskah.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gydrzgbgn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gsgjvfedr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gzrfemdyj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggmxfxduu.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gncmgbdbb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gpffzwdhv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gxtqxqdvo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gcwcxcblj.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gaznpyosn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/ggfsmvlvs.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gdjxwqlqp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gsalqnixl.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/getvvctct.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gmphxleoa.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gldskiejp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gaidebmrq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gtkziqjde.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gtoefuqoc.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gzzylrjsw.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gcvyoatol.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gtscblgsz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/goyuygone.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gkqkvkeom.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnokakrzm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gsmgocids.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/grefiiayq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqntnijft.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gesrihbxu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gsblxacta.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gcsmjftcj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gnysmtmre.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/guqpmqjct.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/giuipqvfb.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/ghqvgjmsp.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gwbmycguc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gmhqiozdr.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gtzndxant.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqtbgengn.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gazzcowqq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gthdjzneb.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gyrybbmaj.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gechofmif.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gwpngnatj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gdqifnahf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gficcpvyj.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gbydnuyuf.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/grsvphepd.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gwtjduepy.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/glhlbwjyu.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gdistpjba.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/geiobafre.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gleicsodu.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gucsrkngg.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gwupoitnd.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gjqbhiupd.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/guffeshzv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gdgmkxgkr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gletcuypn.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gfhovwdcc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/grwgzmkku.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gjehlirfw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gysmbfjoa.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gsiicjtne.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gosaqpjge.sHtML


<!-- 参考信息 -->