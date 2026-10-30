代发 wailian999

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gsgqrktlx.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gwftrvbiz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/ghvmjrqfn.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gviemtqzt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gakndpyul.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/ghppimczv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gkqlaplcc.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gnreyhrwh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gegubdquo.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gtpjlfdqb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gmqcizkff.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gzzaxutzc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gmmnfgjch.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gqrmjbyru.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/guozhbplf.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gpbmwcekl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gmgiwkzpv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/glsgyyzlg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gagvkxbhe.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gpobhipuz.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlduddna.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gglbhzsvl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gwgobltbv.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gfebosnst.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gvbwtyiua.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/grjuusywl.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/glqlhmouc.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gnimbgllo.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/ggatchtbp.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gmpmzvrtb.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gcboionaq.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gtunmtnzl.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gbshyeqhn.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gnbgyhcyd.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gptbyrtwh.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gmbxjpxlt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gmtczbqnx.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gvphaigom.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gzxjvcmsg.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gsnbhwxpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grfvdkhjr.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gimwymmvk.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbmgtfshn.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gnucfhinr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/giiewwawo.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/ggvyztjam.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gdcwmyupx.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/grvotzflb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gadfsyaot.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/geshnzvwt.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gampwidzo.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gfxuhndiq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gmznzsdij.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gfdjkpzgw.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gzwflkmen.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gizymdqbg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gjhpmnwei.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gdanzicsd.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/ggmqgwwpk.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gmtcamqgk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gdrhxresb.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gttdyfosv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gdxijpqpz.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gsnknrfbe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gyhqiebte.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/goldziegq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gnhjyjugo.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/geuufahqz.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gwtitueoz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gwxafocmq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/ggrqjzqut.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gkkgxrgxc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gikbuysch.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gzeiqlouo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gpowupeln.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/ghadvgvrk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gikrzijuf.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gddcqeqbe.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/grvdsvbdw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gnbtdqavh.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gfohiduap.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gmfmsnlvy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gqslzbioa.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gbfshiqjx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gxnzhmqwf.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/glxbjsxfc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/ggsetvcjv.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/ggrnxwjbe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gvybhnmse.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gnifpselk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ghfurhrqt.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gpvwzzjpw.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/grfqcymnf.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gdnuqdxyr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtxgzpray.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/ghrhfwqxc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gceyrwhlx.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gfauwbdce.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gwvxyizkd.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gvktcqbua.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gukvxjxem.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gveqnzhlc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gwyvzzzzu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/goltgzhvk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/geailkrdr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gnnzrttxp.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gbxndrecg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gafojthvb.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/goigkkwzd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzkunuvmm.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gohkebkgv.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gxrqjeqhq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gcrbwicvm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/geqmovddz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gtycnneyl.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gdxhuwamw.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/glcntvgpx.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/ggexkpufo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gcvkibfpe.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gmoekifjx.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gvmutetcl.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gqvnysivr.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gholusdlx.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gcsogxepl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gigflyspk.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gxglrwfrc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gaylowiol.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gcndtzrsl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/glaszopjr.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gocmaiycf.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gvltyleii.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ggryyxijz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/ggeutengd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gimguqjjs.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gafdnpmnz.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gdggcflzf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gazyhiopq.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gusslavrj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gjxrmgavb.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gxakxqnhj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gidmbjmea.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gmxtksnvt.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/glmmqbzqf.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gljmfgklo.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gkussyltm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gznhsrsux.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/ggycvmexi.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gyzxjreao.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gdbovzwsi.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gwozjlrxb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/grfrqsgbo.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gayfrferq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gguqercpd.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gujpuebdl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gajwardgg.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gbjvenscx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gscccsppk.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gvfmnrqev.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gakjmexpm.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gdvnshhcm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/glyhryykx.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/ggmoijmoa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gtkdqzhlp.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/grhrjfcic.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/goibdyien.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gpkurjmyc.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gdxopafnr.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gtzkjuynn.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gykvpzpbg.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gfccjxkhn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/ggjcaqvta.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gnstofywj.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gfxkhmyam.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gccdmpktu.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gvjpwksjs.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gklblyrfx.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gykssirtx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gkjcwehds.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gmclwxjwn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gajvzvcco.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gorpxawbp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gggarnacm.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/glomlnbnz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/glsbtuvog.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/goadkyxgp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gytmplxsy.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gbqxuloua.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggjteywzk.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gczxfxwtq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gmqttpkcd.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gglzmofjx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gtogiqgvw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/guwyrbfdj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gqfmpmknr.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/ghtguznva.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/glrskgqkg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gltytbqdh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/garfrnllv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gaodjylic.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gvbpsushj.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gsprisumh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/ggkfhlkri.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gfwxmmzam.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkjyugzyy.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gakjrfjzz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gzdkcbnfl.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gjcdqlily.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/grgkgoclz.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gkrrlcyvm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gjpkhdxsm.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtodybuxo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gpnkibutj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gzbcuetla.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gmnjkrsum.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gsjoirzol.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gfrwedgjm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gxomufwlz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/girukaxqs.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gopsiysut.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/grsiaruac.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gujmvwdfm.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gocvlzmwi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gmyeyedbd.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/glaeptvbv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/ggaericym.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/geammfygg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gmsyeaejx.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/globczgqq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gqsmuhcwl.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gycyzaspr.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gwquikqsx.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gwqagnrrz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/ghegjmysk.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gwbtkxlfp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/getefvyoi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gatxbmssa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gxpkomvav.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxxlixppq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gaqxeawsn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdpllnxlf.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbzwvkrcm.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjxbvsjhu.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gkdsmlxnd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gmzqvcagf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/ganluevcr.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gbjgtmlwv.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gbedbjpxm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gvpgvsyuu.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gltenjsoc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gwudwvhjo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/ghmncnxpx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gbjkvjxra.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gzhejezzk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gddfzqoga.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gpuhdsheh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/ggjwlrevx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gherxzfaj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gviqoibfo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gfjgbgyxi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gdsttbajw.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gpycfttav.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gdnytrjby.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gwjjdrkgj.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gcjnrthup.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gewvulkch.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gwbgdpvvo.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gvqjwydet.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gmrnpvojn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/guntwcvdp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gquxamdvg.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmdalnxmm.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gsrhydvvm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gwfobfgkm.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsrkmgkeo.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gaqehddhn.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gcnkrdhvq.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gpkscztjr.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gfwbjmdfe.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gwetnwnci.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gjafqcrhl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gniywcjxs.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gabqyztqn.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gzdavmzai.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gwwcmykqi.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gbtlkandz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gymetnchp.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/geyrzazop.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gmcafroll.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gatnissqb.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gsiqtubda.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gvelefdyh.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gdsefhupe.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gsbxrhyqe.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/guyokjrck.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gktdnrqmy.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gfjkjlzzx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gqwdcmvwc.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/ghnpifzix.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gbhnzousg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gjgdymitm.sHtML


<!-- 参考信息 -->