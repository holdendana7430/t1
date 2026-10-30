代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gauzhpnvf.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvhenpye.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzkqqtsj.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlvuajgs.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwiqhtblr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcgwpaza.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/golpzmzab.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gykyygsfz.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxuidcopw.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gtyjgomua.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gemrhrons.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghngyjehf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxqspicvq.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmulppzcm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwgydivnh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdugmtne.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcinzneae.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkdnaiem.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/glfewsfcz.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gegetxbnh.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckyrgozl.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gzcuixacm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/glihptqvs.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gncznvaft.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwwcakza.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gemipmxpb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpjcyjkk.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtnuelim.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdodmaxl.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gmjkdhtgg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/galzkusyz.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/ggronsork.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/giybkmrft.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkbfmqpz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/goocpeujw.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gvegglxme.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gkicwbhba.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gojjcynza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gnexbjnyr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmesvdpvw.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/girwwnzhj.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/glktodkyz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gjztmzpyn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaryblyq.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gbhwdjkaw.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnexicslj.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsupcgoj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmchxlkf.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gwnqifpwx.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gvghwbxzn.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqeczxaww.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbywbpuvd.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gdkjnqzqo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqizzrcy.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjubjrbvx.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gymskcfsd.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgktzkxr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gmajxntro.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gqglqvxkb.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuqbsjaa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlyfomau.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gajnmduit.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvbdirnjk.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gafqavxdb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnvmhilt.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdtkipxc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grrocazay.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiyrvsoy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gtcxodqkx.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbkclobo.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtlesyde.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gdblcwtof.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfmoboek.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhiyxbxb.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxxaxymm.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ggfjvqldj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gbliwzgsp.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjfymlzr.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gzzbmpnms.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbahuqbuv.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gulqpowby.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gghrualhf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmwhwgbm.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gzvsolqru.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gefadqcsa.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gmcbhgllq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnyezvfz.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gsuzbfoky.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gszspzrly.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaqgjaei.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzwqvzwe.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatkvgfts.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfmaotsu.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gcmoznorg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gytlhjrmj.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtahnpazk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdhicird.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggxushnxl.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfmhusqz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/grlozccrq.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxynmhfu.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gbwcfaecb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/giewmwhnt.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdbztjlk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/givipvuan.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggjxjjbey.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gtcyrpxag.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaihnghf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/grgrqesya.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gbxnuljxf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfsbzfxq.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtzxdfst.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/graxdvjpw.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmapdtic.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gihvrxwyk.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gaifmrpwo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gjtufvylo.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggstiuffs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gihlkxtzc.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gdnckrsrw.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gaabgghbv.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/grlxawctm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaokmvcez.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gshjlmvql.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/griddkoms.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcpcgojw.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggibgvewr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghamreaab.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gudkejpjc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzkttzzi.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwonmmib.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfoaavgt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdlduunt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gpkcudjeq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/ganewumlz.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcougfqx.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvoozfcy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclcuerlt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjbjtjmn.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkvprubkj.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkgrmysr.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gedrhqrce.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gbllswtvy.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gjkrmovhu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/grtngffiq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gywwapsyi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gslscslli.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gosqjbinn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gxxftfehq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdydbyycf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizwklvuv.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gobilgtkb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbemenhuh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gflzsarif.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbtzzoopx.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaeptoee.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gkkijkdpf.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeqmfnez.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/ggyjmwqqn.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxhxmiwg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gnmjalksw.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjmyvfbn.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gsagglhsn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjoulwwt.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/goeyeaqvo.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gashfmjyf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/grsuurbyl.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdctkwaiv.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcxzehqz.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdslwoaug.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfppkxosx.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gpnootyui.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgfogutj.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gbybijpoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuykouer.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/guogiuvdp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gykwgpdag.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdmohvuj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkjnpvlp.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/ghprfbesr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gigajbdll.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giijerrmr.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gdrrtfnau.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjmsqwpi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjxcdjks.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjsbpqhm.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gtjxxqmzf.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghocgcoav.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbpqiojp.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwpkyxbg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gadzvtkdj.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/giairjqkw.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gcvgfgelk.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gxghrlgru.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhuhbpbp.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrljggzc.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gycojhooa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcngfjvb.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbqvzhjkb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqlughxx.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gggfkrncq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggonjxjzo.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/ghobheisb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqiolaznv.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gsxyioolv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gizglldnt.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gedmthqom.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjggkcttv.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gkftyxleu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqjdtgfe.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwozwvepa.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gjliltevb.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfbhdttyr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gpgzobbrw.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gyhqiyarn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwxcjvkt.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girwiirbg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumzkaxgm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnrailhht.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzugftadh.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/girafnvcz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gdenbbajh.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/glhhbbwrh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gipdnfqwz.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxbatczi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gvhxcqllp.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gieksinsc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcpbecqa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guglkiilh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpfinekui.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giorqjplx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gwbbcpnji.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyyvlfqy.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfopgxej.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrorgmju.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gerqlxbxg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxodawngl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkrekiiu.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gudwmajui.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvvtlgnv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggipdqtru.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gutmeqtfp.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gztetyntw.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gysxfgrda.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxwneaxal.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabnlcsur.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuuyuwta.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/grwqhkuvh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghhewtxvi.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqqtlwms.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gptpmdrnk.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gdceqyxct.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gnmvjfgtt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwfiiqpx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpitgglwd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gdwtqnvdn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsjgcucc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjwijwcgs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/guiklumkh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryfmizcr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcnojnaph.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gasuhndap.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlupqfct.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gnvszybrj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsbbhtfi.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaginhfmj.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gfekkqdhp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/goysgzkja.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynzogvtk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gdrmaszut.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gspxtzotf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdnovnie.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/glqxromdz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gfykkcgln.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gphohqovc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gupcrsuqy.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gogvxpnds.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/ghdjbciez.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehdwdogw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gkdjgbzuw.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/guzfjxdel.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gpexdbrha.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gqvnumfth.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvonlmuu.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvelgtig.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/geislypdv.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gpbryommp.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaxusxpv.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gsolqscsi.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsefavjk.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grotsxjel.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghjdkdcga.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtehvadfn.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrdiqwyt.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gcmczxlpz.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjywdkzce.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcrjlbqu.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/grnfcbwnb.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlrphmax.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnybdcxho.sHtML


<!-- 参考信息 -->