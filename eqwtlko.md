代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzmshqqq.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoilqfiy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpngglnbr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfqufzaw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwvhxqfu.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gshwgsihp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrdvdgsr.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdszoptk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gphqbzglc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvzwrqdh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdixfphu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gledbnxwe.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/giduxkxrq.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclibyuim.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmwsvnzky.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gxpjuakiw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnalhnld.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbnuuhqx.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gmhmfstxv.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gtluklzzu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/goulpuxcu.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/golddccgi.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gspyejwmv.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlqhltas.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzozbzne.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrszrpqo.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gfmzysuex.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gahqxtfdf.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gklgkyolg.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gspyltjlj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gdkcombao.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gocyiaxny.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gywtqecnh.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gahvxznwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdccjcnps.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gflcbmmwu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymejophk.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbmezstt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyfvlkgp.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gjkizuwig.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gwjwooleh.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedxxsucz.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjooucben.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkavbwxc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gkjxklscw.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcgpcviyr.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gavcvvtwg.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gaczqkmds.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gkkwaazpf.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gtrjrfwyh.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gzegvsvnt.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gubxzpumq.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsmsgytk.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwciuogjz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtlldnbr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqzxwkxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gfowjqjpf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrhtobpd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfjkwcny.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gjweuncim.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gqgmcrzeh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxwzevkqv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfzfajiy.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsezkfujc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gdswstwiv.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gobjojvag.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrnymfzu.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/grbdnotwe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqyllqiw.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gaphkrnzq.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gggbpczoi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gzklqiqee.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuqpbrbr.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gbybhxhag.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfrqqtwv.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gokcfckwx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gefypcjjp.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbxexcst.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gfqmpitod.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcqiibox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpcpjkdz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/glooxnwwc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxutvjzsz.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gojcgznbw.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gfyzkiewl.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdbbsvfo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/githlapzo.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gagpmqhuu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gjdwisdks.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glbnzband.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgorbclb.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/glpjdrngg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjmudpfp.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoovtign.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjyggogjw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshkutalm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkdmizcy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxjamnok.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gancewdzq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkoylonz.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gmnviycyo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyyezuhs.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsviycqma.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gtpvgcbpb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsclggipi.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gylhvfkmk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gnbiwfych.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngsybvk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/glmojwdsi.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gnljxpqmh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gfeaffayz.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gztdetofh.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjsovjxyh.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjnxrxnc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gounjdtal.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrohoszq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gtqtsxdaz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/glonncdck.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkbbcjrd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gdrbcjrdz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfmjeebu.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gtqtdijlc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gygomxrok.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdkyfhoi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gopopfvoh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gukbwiqrq.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpybwkqr.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxxtgrib.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/guxahyyik.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/guogowndo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsubzhlhq.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwhrbksp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/ghrcxszfl.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhqjjitm.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gnwjqerdm.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmjoemrq.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppiqpdxk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduallfxp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gcnfwgqxr.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhdjayg.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsrwktta.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glgnqobnl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gezjsncsm.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gohysatei.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gknamsvca.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/grolhrvmy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqwsgnde.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/ghnyyfrom.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnalunoie.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsucujemf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glziuezsn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfhhkhps.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gonrlbfeu.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwqchhxsr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuahfqmd.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkxdqsrn.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxoreqoy.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjsmudqhe.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfecpibbj.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/giwdvrvje.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gojwfyimb.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdttrxpq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnyzhjeh.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/godznrzpr.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqzfdyita.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/guexzxywc.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdrpgudr.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glycxqlid.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/giuvseerv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gayncuwcu.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgousumf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkorvkom.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdghomub.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcgqhanto.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gzgfqwwlt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnkaxytp.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpktnucoa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmdlhqffs.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaxgldxg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gedsjqpim.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gdpypbcjt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpxcoxacl.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/grzxomjri.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gtldkmkyj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gqisvkpmq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gxnlxuasq.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcutolqhk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxucneea.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaqdfobjl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/grpqnpfsf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/guraazpvi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnohvssz.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gqznvzrgg.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuarhmwl.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gyhlhysex.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmmiqidz.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gwodaghma.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/grkwiqqmi.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gklqcxblr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtsfflsnm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gpzqwojib.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrtpahxk.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvedpsch.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gorpqectd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/guagdnyqd.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypxxfkpn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gsakvptfh.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/garhugkul.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfhhtgmm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glggjucal.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gouxuujlr.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gsmeaflth.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gypkxlafj.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gbogfwnzt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbneqzdkl.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ggstjnlbx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gertrvsus.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubfdnzoi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbffuizj.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gipxiiqug.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxkclzfy.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxjzdrbi.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiiluuwe.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxvqifno.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxxfutxe.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gawebmlnj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzppmwyg.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gcylmlugk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gohvfvlol.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtgwxajm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggllefmcl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxfoqrit.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/geihacdvw.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glvkihmpj.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkuimpzbp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftdlisyd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboxczhyh.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gifdprlkx.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gorlncmxa.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gjemepaho.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gokmnorrm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcjcybch.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhozatjj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbwrrluci.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgktblym.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfneoxqx.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/grycrjixh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gogkgslvp.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gykvailbf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjjpamhf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gvazhwxjj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gihhmuqoz.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/glludyqaq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdpptzuu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/govkbqrtj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ggpzoootd.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gevmtusxq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grogxekro.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfrzasptk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guawidcbk.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gofkxkzdz.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnrjlsdu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpnozdov.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gthpnkehr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpfuglig.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gniyphvhv.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gaimimxhh.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gatdozuxb.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfmvqcao.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyycungx.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gogeuzqsc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gryrykrcy.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcevmadl.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gdstbydmj.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gajhpdtlc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhdbvlla.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/giztcgdfe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/giaaegaxs.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkezfdji.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoimnktj.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gekfxhbmq.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbwfcsqu.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gomujbyst.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmkovedc.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gqmihipcl.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbovcujnf.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gldoiqnup.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbicvhdox.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/ghykzkhay.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqcsqanl.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbzlsssf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gybvkfjha.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gklhyefop.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gvbageofh.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyncymlic.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbtwqaig.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpdccnqw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcvivtaa.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxraecftv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiyizkds.sHtML


<!-- 参考信息 -->