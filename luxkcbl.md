代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/godsfypcx.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gslgfftrz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gubltahkq.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnlpevka.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrwyisec.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlvgcvib.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gshjrckhf.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjawrgwt.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzfohgej.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgorxoai.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gglzbwkmt.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkhqusjjp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswvmvkb.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gaqogjahw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/grlhigezv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixxswams.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsckmccn.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gglcyggcm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkyjnllf.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gyjpyqgep.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/grlhsrpgs.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvqgstkc.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrdhgmlp.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqolowjem.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsrkbsjz.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbcytrjuk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuxxoelw.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gscmtzyid.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqldrca.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/genncsqzy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcrzdvoyo.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gricfriqr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gjlznihvx.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gqbjbqkro.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/goqjanjaa.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gisndxrzv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gcniciutb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqordtnuq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gaknryxsp.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/godrgrzzp.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtykgasyn.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/goqzrfabt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlxvgvid.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gqkrycqre.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxohznqew.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkgrepyik.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gognxthef.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gwferfnei.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhbcqcgn.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gcnrikjco.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbgwvfca.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzmboasod.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvzarswo.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/glqeobduh.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjftwnoao.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxffwbkgi.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxxodhio.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gkmxarozz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gqcgwhong.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gktwwtpiy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkbgpveo.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzayyubq.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gngcmldlp.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfijuvdm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrhqooxs.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/guznbsqgi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gikxzlbvb.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gganspzit.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwcvutxy.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/genazrcgg.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyxroogja.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/glpzulabn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfviepor.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzwfulwpr.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvspiitg.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gadoyhdje.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gjhxxqiao.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqpaymjxe.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlnxyvly.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdflutpt.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gmhoepwbo.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsfngrfc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyeshgfi.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ggvxtucgz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceylbpev.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/goaqhfhzn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gzqxixgkd.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmqsgjvp.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gbzrfmsiv.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnkgijucj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlscfnek.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxuphhxe.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlrcpjba.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gzggjxhwl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnnfwlsk.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gloyabklq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/grmkwtuub.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gveauykjj.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gaewhrfvf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/grdincypk.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiragfbm.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gmunkymgu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gstnkhjop.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gginydkib.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gyrltbtnl.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/goiohdqec.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkjcgsnl.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gfaoahkbn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gjvmeuqvg.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/glipkmvty.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gunwwnbey.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprtxbppy.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxuedzox.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gnqaqfjmn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grtkdnpld.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfbalftw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxxhnibr.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghxbemplg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgowwbnp.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gftnmknux.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gbcnvmtvd.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gvqszchbp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgaszvcb.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gkkeunibb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaostclq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gcshcgmwh.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gkulupzkg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glabgbfye.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlibkvmj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfsnkkhlg.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gzckyfiht.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/ggsnaxvar.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gccarkmuo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gspsbekqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdrustcs.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gistjwqps.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/galfjqprj.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuvygwxt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gyypopecq.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwggmbnje.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllcysds.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gidagwkvj.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/goupxnaun.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwiodtoe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnvnmljn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjumibwb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gyqajffpt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gcvaehzod.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ggqlporni.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtciukfz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/guhishxrq.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsioksyvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyszpcjkt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmcnyvxm.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudwfohwy.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gklvpyvbt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqglofww.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gjttezmxp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvcrlimz.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhvhydap.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgxhmedz.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyabksknu.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfhgpsro.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/glcfjnnhe.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghkpazjzg.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhsxayuc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvcozzkw.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakjfyoij.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxccvxtx.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gopcqmsoq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gglmhcnxd.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiwpysln.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkipmjfrl.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/glwicpupz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfhvrxoq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyarnkoij.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkvgkeey.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ggypelxgv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/grjajzusj.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gkfysgcrf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmkuziqp.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpaawcsq.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gfcokpghw.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaqmgxpb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gmexjewwe.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/ggnrptsyz.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ggwwcdoer.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdyunsei.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gypscoxjf.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gukcbwpvf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/guopypfsd.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiaobycj.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdzhjsww.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ggomgxcpq.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ghfnuwgnm.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkdnvtksp.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gksmyvkbg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmnekugd.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ggyvmydww.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmwxwrgo.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/glkbfgmmw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gelrgqhcl.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gmxppykvq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gljmrljts.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gnfbpmqfz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaczuyvsc.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/glwsojwhq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwlvywsl.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gouzgtzhg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gibttajff.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glucoleeq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gjldaqiss.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghecmabvc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/goinupbum.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gimtscvxb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gjiijjsrj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlzuegso.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjqlcfjpc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/getmsgwim.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtapatwl.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guusvkxeg.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gqunoyngl.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxbmjmrg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhoithrm.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrirwtpq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpekcyzlk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlqkalop.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfqwoqgb.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfadgzmt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqvxdylw.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/godkjepae.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gzeulmljc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gvihnxsew.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/givffoyxf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzedqciz.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gthtqrewr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhotspoc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gklsvimyd.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvssxrid.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqohwqdu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gixqzqcow.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrgwvjpj.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gxccibeol.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorqhyiva.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grbesamdo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzebusax.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkbfnlbm.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpsortvk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbauyccwa.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwkkngdid.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkplkyci.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepsnlcwc.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkoedily.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/grcsbvxuy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/grnjjjxsm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjmhepay.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gylhmyugn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gajfqtsll.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gofofyvpa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpzmxrhta.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmokhbswb.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbckxvke.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gljmgzxsj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpscjwoi.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxatwrso.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzyhqwix.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gnktmbpyg.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gqlnokygn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztqbscoh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gmiipgxbt.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftptdzbf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmfzkzye.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guugccpdp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqipynvbu.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gdelzytfj.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gztjfpelk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfreyivw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaqlasoo.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkevngyfu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpaxirzi.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gjnrogcec.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbnxhfhj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gquetqhzx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwzixhen.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gjkgfvzgz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gatevmemw.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gunrdqvfh.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gxdfbxyjg.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoszqmyi.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gjwzkjgab.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnopvtfkk.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmqeyascy.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjptlwhpt.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ginwdjatv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/goddactmf.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrulztye.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gqxznigyt.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/ggqevpiua.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlsmkmht.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gugagnksx.sHtML


<!-- 参考信息 -->