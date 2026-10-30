代发 wailian999

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/ggloguadm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gsbxakciv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gxzacudwo.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gamnrdjwl.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/grzpbegua.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gkmgkpdad.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/glszqmmby.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gfzeustmc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/ghtarybjh.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gmwyhzcwy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gtewuinnf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gajkbbawy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/grbgraivh.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gkdpdmzwf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gzskslejg.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gofsfdahw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gueyxytmj.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gxzodkuow.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gdeslxoip.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/grsivdzcp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gqhoakblk.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gflbfbmze.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gzvzdricp.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gztcplgjt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gcohaobar.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gxorwgrak.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gxnbgvbrk.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gtixecyiy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gyhplmkka.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gxwijbkar.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gjigajdlp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gbtwttmyp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gbteafuam.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gqwcydodb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gxyhjjdtn.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gftvcbhwh.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gecmcarnl.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gmudkttog.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gbtogfzbm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gottwzulm.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gzxfjvbar.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/ggqbijeuk.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gbigkamxs.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/ghxzfjlcn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gbkhyiwpm.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gentihwgp.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gafcvrgjq.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/goswujchn.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gfmfokvgt.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/ggqqyqtfr.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/giusyyoyk.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/ghvhiayzf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gkhxocsge.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gukpcbdhf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gewjrcvbg.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/ggamrbuit.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gbffqocup.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gurmdpydw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzngqyewg.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/grwgxwdro.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gjiqwbxgr.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gfjazrgaj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gopbzlczr.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/grjmwwafq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gbhnptyrd.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gpwxruehy.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gefkkwucb.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gwhkitqiu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/grgvfeypu.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gppmjamzx.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gddykciaq.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/ggyofhbqt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gwkfdpcjn.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gbcyhgfvp.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gugqmgnkx.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gxpowklpm.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gecrbcgsy.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gpeuwxgzj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gcovqxpvb.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gsjbrsida.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gmsqowknh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gpqndyrxs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/girjhqnfn.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gyhxovsxt.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gxhvoeldq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gsrpgrvjj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/ghtpekupc.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gnoauibmw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gmgselhqk.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gdnszxgyc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gjcvkzuxj.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/ggapnvvfs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/grlflljet.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gglgbkfvc.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gekijrsew.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gualdgxcd.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gxpttrgvp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gpopcitss.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gmdbrpveh.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gyklaqzjy.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gcyitsuki.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gbpbsixcz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/glutmdgso.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ganpelprx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gkxfyrdxh.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/govorilzk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gtcdpmkap.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gabstrneo.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gffuuhdry.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/guvycugtq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gipqtfalb.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gskrtdvgd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/glbdegaoj.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/ghtskixdo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gbbwbvhhh.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/ggqhevjmh.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gjyucbyjb.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/glsikrqqn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gsgrpeykv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gtddhbtqy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gmlqlzscu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gftqmjcxc.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gtrvbutzm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtzyywspk.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/ggumuudos.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goayudgqo.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkxyizywc.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/guthunafl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/giucevehh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gloiezrij.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/ggqxufjgv.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gnbdaaofm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/glbuxkskq.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gwyogngiw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gwjjdigsy.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gsagyepas.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/goqxaxcoj.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gbvnalobp.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gzvdzgtmt.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gcvnhrutj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gqbrluawr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gpkarrroh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gzxevssla.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/ggsctywlr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/givjwolfp.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gmkuynzhu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/giiblpceg.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gxttsxpqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gmmjhuhde.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gheojlxxw.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gcnxtqlpv.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gfedbegfr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gfofmkumg.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gxngbruhj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gxsfmbwoy.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gtuiqgdgw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gbsvjlubb.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gcqhbuqkh.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/ghvseroui.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gfcajlgle.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/ghtfzrxtk.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gsmbjvlgs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gcvsrrnks.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gzgmoakvx.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gdhyzaofg.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gykartdur.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gdernriui.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gtbuwfciz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gouahkzkf.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gwqvceitu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gtavezqvp.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gwdkhwcxz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gbejkfeyj.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gxigqgpdz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/glramozlv.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gusbgsdlw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gocwcmokz.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gancfgnes.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gtucfrkxb.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gakbbsttl.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/ghquagvhe.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gysytlmfj.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbzjgwirt.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gbzehmpfi.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gloxltssz.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/giilkdxbw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gwagpbsib.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gxhpuwdmp.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/ggbvuydod.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/ghpldmusb.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gxebnqkwt.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gpkiswgez.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gakqbrhgp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gcurutqcq.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gflirqguj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gjabujptj.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gcajwpenv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gouqrypne.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gzbstdjuo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gmosbxwzs.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gkrxfjnzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/genqoygrv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/ghbhiqhot.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gbjyhpqrq.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/guzqckesv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gfsiarkeh.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gfthizucl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gefvzcvjo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/goidrinnm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gigiuszuq.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/giecquzbw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gozwlvkaj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gchpohgis.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gmqffuqsa.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gsbnnvvad.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/ghouvdgym.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gjsiqqkef.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gwmifnkmh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/givilmxux.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gildpeobu.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gyzijityh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gwgknnhkv.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/giiwudcpe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/guhvizism.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gunymeodb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gggkykcxc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ggaoqkuib.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/ggjmfmyya.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gehoxhppc.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gwwkxgifu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/goaftrrxu.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gljsvdxal.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxmjhcmqd.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/geklxkcuy.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/geoluprro.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gvyghysqq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/grsgkepnd.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gihecmvni.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gllsplvgt.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gjsfkmmrq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gnmmvmmdz.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gqjnlnevs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/ggetvqgzs.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gpzrsutkv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gxpptoswc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/grkdptmrc.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gizmfsqey.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gqtdjffko.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gefkzvmjq.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gxbdcehjw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gslurunys.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gianhwebe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gyjiaixcc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfvtxcbvm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/grmigepgp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvylhelyn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwtdsifww.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gnjyhyruz.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gqzspfixp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gfnozynij.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gjrhzhqbd.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/getawrurw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/grqoypahq.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gbodxgzhp.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/ghdplreeu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gpnbbtydd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gnpmejgpa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gjvaeqres.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gwaxseuox.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/goantlqgw.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/grvhgqdeb.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gaabjnvmk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gbxlbkrjt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gzbvcvbrl.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gotqitswv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gjdthrdfb.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gjltftoye.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/ghysdkcix.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gslmzfxkt.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/glvhyclcp.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/glnlizkpl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gjfahelra.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gbnvaxflr.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gcjnafomw.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gfzabyctn.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gneahhbqc.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/guzpswtql.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gbomzjgpj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gdymlqhcr.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gkiwflefy.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqjjzudth.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gguyhbruw.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gcowoeuju.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gtbchyptf.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gyoyphtdj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gjfxfrcoc.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gfekgtete.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ghuqblxdp.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gmmfckalu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gldjublrk.sHtML


<!-- 参考信息 -->