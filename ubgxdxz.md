代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gitpfbeub.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/girpjrexx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcfnpoeu.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gihxebsaq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvhdwduzj.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbugnhqqt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gauqyyweq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjjbgahtn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gyasqvaow.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/geocovdsf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipozobcm.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkquwfox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gzilkunzb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfzhmafd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/grloustxy.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftxeupyf.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdhufezw.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerqzcdhm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gobciprep.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/ggynzzvgp.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gsnqssnow.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/ghubfxzao.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gkfnqrxeu.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/ghosoehhs.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxqimncp.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gcywbqolc.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gazjunvry.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmdjjfduz.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/glpnjgcww.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjygvfwz.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gxavvmajl.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/ggunmprkq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtbvjsss.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gdgmwsngu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gasaidifb.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyhyiodn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzyedaafe.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/glxlictuk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjhrspim.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzkhowui.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/ghbafwxhh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gffnkleuv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpiqxghst.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpynchapq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkpepddn.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjwenxip.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gojmzgxhq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gnijthvao.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsvsoxxp.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/glnqqqrfj.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvceoewhb.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkudkhlp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjryhijz.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjjmcejf.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkkjpakz.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjbeixhs.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gclzimttv.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzqvhfyql.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gvjdtagfa.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/geodddhtf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/glzmkdkuo.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoempgdq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gnowomvxm.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxpvdqbi.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gnecgalay.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guhamhmaf.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoudctwy.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gogwyhsdv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/grdicfbwr.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gprmntngj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvreitcn.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdncteqp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gzecfumdd.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/geeeyccgf.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gxwnenecx.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gktnrolaa.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghpmmlyl.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqdzavak.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gztbrfaez.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvanfogtj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxehsynmf.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggvqbbgok.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvdxkyycf.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gffrcheox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzjqfbyp.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpoqbmoh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gprcmkisz.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvaoivpa.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakgmimaf.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gdvihbsiz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjokwqzwc.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/golqvjfsb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqoukwel.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfxmhscfu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyobomop.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gekvtczgj.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcwzcste.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfmowplj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmyntfnd.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gwtnykpvv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmmnxtcp.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gjvezvwak.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqpvqkuc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiyvsjrt.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gpjxvgblu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glpwkmpjs.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmprclbuv.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlonlwnv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpkzdoob.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/ghngxzwpo.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgrouegf.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gqfpujhxf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwofsrwy.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/grovwfptx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdymmcsxj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giznccwpq.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcbtguqow.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzvzqbux.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gyhyoqyvb.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gailjszbt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/giynfdaty.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnikqpfb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gavrrihlo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gsrswpyjl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsffehwr.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnamtvab.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwfbrnxs.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpetnizl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltmjoskr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gssppvezx.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gfmcsdnik.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnefqhiby.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhsimhia.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gaesdambs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuinuvew.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gxusbeufv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxtzydgm.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gileteojs.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giivyhtnd.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlvpjlyq.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/grewkrhhq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ggwdykrjp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpcsoqea.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaudfatm.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnynqltu.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedxlvqyt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyjnkdbo.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gghtieqgx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqekzyfso.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/goikktjcq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpkpnwbb.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gubyjjnqq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdbzivjm.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gicintxhj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gwhdnluah.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcprgjsw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/grhiakmgt.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbpuyuhvr.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeenjhub.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gslwssbts.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gxibmwepm.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/geaiyluox.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/givbjborj.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdpktzvhe.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gkzggwbfj.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelnrewhk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtkvgtl.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvokuckp.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gfsvkxwbm.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gymlvgnbf.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gwixkdeuu.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlirrrjk.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/golwzmwpo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gedsrhqsh.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbjakowu.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gssxeinho.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdjgplxp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqnzrbwfi.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gecbrbdyh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnsftntby.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/geitbggbh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grdbcejrb.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gynbevcsu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmujnnhbh.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gebmfiswb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaozpnvg.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbiffzfrl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gicjtefcu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmfnumhaf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubcfnfem.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdryltylw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudpoibee.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcmepyeon.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gatgjgbni.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqjlvoes.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/ghvaqvtpq.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpykrwprt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcwfxyin.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhdnmnck.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzenldmid.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/guflakykc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghejosvvd.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgaatmbi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzbfqjivz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggevxqhub.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxdkvlyx.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/geuszcwjr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjvnhnln.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflbcvdkz.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/glrkvjyba.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gmgtcbdjh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gletgrmgr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqjzxdihk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/giygzffzm.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gyeyopduw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuoiskux.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/galmznxqt.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gevnzrask.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/guzegdgfu.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gnbyttequ.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpfanicr.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gojntkokr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/getuwfbxh.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqbwbxqu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/giujljjdg.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyibpjvel.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gwyllcaxo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokiqotdc.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjriazmh.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbaebuoe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gyailmpft.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzlvilui.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzhlfpzq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gelattolw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gafsprnjj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gaakalfvj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnqflrbtp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gcvdlcisq.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gpksiubzg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gdmjxwvcw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgpxcmus.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwzjlnoc.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvbruuky.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqvetaqr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidwabdej.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gpfjgbxux.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegujjxqu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gckihjwks.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvyvkfdh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gmgjwhhue.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwwqrfsx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfccsbnsv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxjelgsb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyfmqdsm.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbhcaluch.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gtxlnzqzb.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnrrymxt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gllkoszko.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjffykjm.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/grfgkrofs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gujnayoog.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glueftscl.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gnwivrbyn.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gujfjorta.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/glfvpzyyy.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuxbsmtx.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfcptqlrc.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gvacudlfl.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gbzwurtcv.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjfiaaugj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmitrdczi.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfmynnsg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gabgefbwa.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gofftphbn.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqkbperg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gigigsqms.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/goueorpxl.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuwkrqwe.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoichghn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gaanhtfrp.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbobqcyym.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/glwwgizqc.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gvpylvqrq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdprrjrc.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gnxvkcdmu.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gkekgdxqa.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobdxincp.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gouwxmwwe.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/geiifnvrk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gftqyyefu.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gwtumsmzs.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcztadcrs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gphxaddxn.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gnfsligkr.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gvegzfivs.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxumgmakw.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjqakfudm.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/grdadhivb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjqjukkj.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/ggnfeeasc.sHtML


<!-- 参考信息 -->