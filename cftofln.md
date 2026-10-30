代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gajxxtbln.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/goksctxkk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gawhssobv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfvuweww.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gloqqfytf.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gtuvgtvgo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gluaflzdw.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyaulsmp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gsbeuipnt.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gtdqvqanp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gerisqhkc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvgmtnox.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gyydnohyt.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwsqktwy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gxatvqlny.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gdvilubdx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmlbvfkr.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwrfqridz.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjsuepdy.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdayfaevz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvrqbtyn.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/glfrjafsn.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gspzrbjpk.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkjaqamrj.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjiubtrm.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlihxttr.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gwrbgzefx.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtthhiac.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/goqvjcbyv.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gzwadphwb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grncicdtg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctpvkukt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gaglbffyo.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gdmjfmpjq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnhynggg.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqmtxjrrs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmkrbbii.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gavbmtulx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtxurbxw.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcxuohtv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxecstqnk.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/godxzcwcl.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyipdpbtc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gukgsttga.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcquipza.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gizlyjexr.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glesnxvvt.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/goxwsgsez.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuevhnzu.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/ggdycvsbh.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gtohwmywb.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyjcpzln.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gasriuuzz.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gworasbce.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gpljxwbau.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gcamfyhze.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/glzuitjms.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gocooxmgp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gbbdpfnpq.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gykwmudju.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gmldpmjxk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gifopbmsl.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gugaktzpg.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gjgjofcka.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gnmdalznd.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/grvmmxhcb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdujzrxf.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxwqqrff.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gynbibvnb.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/grksapnwg.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjxbzlqsu.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gnqegwmkt.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/guatjzxcz.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gizcmormr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtpobiyd.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbipivlco.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxickogqz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonmaxqtd.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gjvkebyoo.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyopbshk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmyrtyuw.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gepwyfakh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqrjscgd.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gvotfngqx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwqzbeba.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gaseeyrbz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gawudmnot.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grenfhwqy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gtucyarta.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/grweeucdv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/glckyjxms.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttsagitc.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gtzclrdtn.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gulfugdop.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghsxkxnlj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqmdobat.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcfmvrcev.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsnrrcsl.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gtnyfsytl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjqdjubq.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/geiinoeur.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gllxcdqys.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjspwahv.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfaudwfq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbaybaie.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/giauehgfs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpdxoune.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gntyumuol.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcvqhawg.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhxwozkz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrlhqoux.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqdcqrpm.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlpnlqjb.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqzgfwwxk.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gfmepujom.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gldwlkkcc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeuilkwb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gahfzywqp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gelbbsqot.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gurqokbdw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/geykaaonm.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/grukodvhe.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmnkqwjy.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwpclxznx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszlxqchb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gulxvknzk.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyzvayfy.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxhtpuwf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkfiiyfq.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gdyzmraji.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/grfpqixmc.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gaayhhyle.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/guqbnhnis.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/giwtvuhon.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gpskukykt.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhdlikmf.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gpxstpdqg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyrsemrn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gbxmdzjwk.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfgnlmqu.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gswjcjlxc.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gulrkdebj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsfsyulr.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/giwavrukh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxhjocco.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqlabitj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzlkqbxu.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbobjrbcb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzexwcnvq.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnbpmrvk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkhdjjeg.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gqdmmahsj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwtsxltz.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgngfywn.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gapjjpgll.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gqsyrrqep.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcudxiyv.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvgcykep.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvznksxe.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmgyucwe.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/ggvyiwteb.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwzfhej.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gizhrtsbc.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrxvgytq.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gwysplski.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gmqrtynpp.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gruigsjvi.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjsravxw.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/grriqnddm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gftyjbabu.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmjwtiuuh.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gohyfqyfe.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/grqcueknu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrmtubak.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gqhxzcwnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gblmmsnzf.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwuujoay.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwamrdkbo.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdpxtopa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvttbucel.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfeogvjo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuhvnjpx.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gllvbbrkb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gsqhqbwfh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gocqbpijx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gqxlyxkbd.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltjlkxmw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpvqpoat.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgmzsrxi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gyjudkvct.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gajvtwisf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmxzfedw.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqadritb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gkayvhuow.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gbthjarlr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gugiwsexb.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gamgvmvyt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqfcivrdp.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gjnoscfcm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnnnmtys.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvxitqqap.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggplcahvz.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gymofwssy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gixpnsjbm.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjkismuyz.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtenczccd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gdufabirs.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtunizzbh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/goygkboua.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcqqurxqj.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjpozfgm.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gqropbwbs.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgrrssjp.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqbgizkk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgzlengu.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gtcbpxhbs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcilrdgcv.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gqxystpzp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gafnvuvaj.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbztmaxvi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grmmlueep.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/ganougqsl.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gwhrdcapt.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gtczpdqau.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpooqcyeo.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqaxwfyh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gsmyegwqu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfaghdja.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyzjfvsr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grykbeocl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvgabrwn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhvnksmq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjgswmuj.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/grtlgrndz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqbvxwzp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gwsvwkjrx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/grrsflvpj.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gceeqwayk.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gpcifriva.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvtpwmzk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcdnjwyo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/grfrnddyd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gdvthanly.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwebwyasx.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtmqcivwz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gojsepeya.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqzezkju.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhqknjha.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxfyioyu.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gnhauemwk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoopwjmj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmxzpqdc.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gozsxfrmj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gandkbldi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkiahnan.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxaqkgpdm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ggblpxwlj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gowwlrmir.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/giczonuli.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gwxsndyea.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxvyvgpu.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gsgsucyhb.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpbrlaih.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgafqjhp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvwngggk.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/guwgslsib.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/guykxvkkn.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvkvqrru.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gwxkyhcus.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkwygazje.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gieolbneg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gvyewbhch.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlrbdtvq.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/grvwxqxpc.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gcebqxzes.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gbteymotu.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gndmcfppv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmuktlao.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/grqqlgdsz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gdgkdkuzy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvcfhike.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkbfbmcm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblcyzjga.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gdelgpewq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkraqtlmh.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwigibfw.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gyznrutre.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gdmsfalvh.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/ggncsjlvw.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/glpnzyipy.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmvzzsiq.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gqomuufcg.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gaahvxnzv.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkreugty.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gliefmsrp.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmvqakvm.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/grddnqdxl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gglsoqkvs.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeynzdvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gjtidsbwe.sHtML


<!-- 参考信息 -->