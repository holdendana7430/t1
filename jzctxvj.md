代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gvzyiqryq.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gmpojfvzb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gaghlcuzy.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gmqfzuepo.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/geywhecwb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gmlsmpwxu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gbodoowyg.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gdddjlmyy.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gocltxrgo.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gdacmxakj.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gydvrtqal.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gjvrffjxt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gayjswxhh.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gcojbqsag.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gqsjiyxzx.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/ghxbjdsrg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/ghpbictae.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gmgymgepa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gsfamvjmr.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gnqwoffpg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gbiqqkiuc.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/ggqyvmobe.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gnmspgost.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gcxslooux.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gnrlvwuas.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gzywlwiqp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/geghvvgfv.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gycdfkvqc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gzdhplvhj.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/ghamerhxs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gtahvdgwu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gkoeivghe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gulykpqiu.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gnakqpfed.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gkvmxooeh.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gkdqaeqvo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gmqvoolep.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gyunhgnqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gzucgxyar.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gecwtplxt.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gqojvuzde.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gbomztmto.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gbqcnmajy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gakhiweqe.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gkcgvvtyl.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gnzrmfgsq.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gfxxxgxfj.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gssjsjmtb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gpasuwztw.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gbgcokoic.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gkhenjwvw.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/ggrthqzsb.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gknocejup.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gidqkrehu.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gbmhrflsa.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gzqhcjgsc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gytafqzdq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gdvcbairp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gknaumgep.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gbhrgppon.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbwtvtdnw.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gzeuszwcn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gljfviyyd.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/glfgndizt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gygvvqepy.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gxbapcvcr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmjthjybv.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gobpxtzdt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/ghzgnbcxs.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/glbwdaubh.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gcgfolhuz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gplrzunxg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gjilcqmsp.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gfqweobit.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gkhquupck.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gllzihvtg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gzdunaowc.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/grcrxugyd.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gjimwyony.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gmbxogkmv.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gitjwopcm.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gxgexlezw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gqyzryzrg.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gimiyvrxo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gwpanprng.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ghsorebrx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gpnocsyfv.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/guyabrfci.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gotrhmgoo.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gbikcivjb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gfeqkkhzo.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/giagxigbt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gckhkcyey.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gshfiuhbx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gwgwoyatm.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gijimsmmc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gczepiwhk.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/glfqgghwv.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gpcdaqagd.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gyhpwfyyj.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gkxpwmyph.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gutbopsdn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcjugxvdz.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gwooynpvz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gvifokyxe.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gyjzrbnbz.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gimtxcpfw.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gtvxdwuwu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gxmolcwpu.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gqkvttvyg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gotxlpkxm.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gihfkgwba.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gxdffwcbb.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/grruyhavq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gythcdjay.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/guqrffldg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gsmbydjzf.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/grjpnhsnq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gifstvmtv.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/garktjsqi.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/govbkhgzz.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gujvgiqlm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gqjtlmsyi.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gbibldfxf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gekzgqlqk.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gnzaajeqs.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gzewvjoxa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzsnzrbdh.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gijkuujbf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxxbjvtoy.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gibftxmxg.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/ggbjhvjav.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gfuvhidpd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gabvtssag.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gsruflfet.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gcxjouied.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gixwlqoow.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gbkenbgxk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gnjszywej.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gkizbvsvc.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gdqjwhsme.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gigksddnh.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gluoccoxw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gutyigouy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gofnbxons.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/goaojsarx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gabmxxopb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gkusnfhjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/grlceeyka.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gzaajqryq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gzaonjcau.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gclugqleb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gaubtkqam.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gfjfstwyd.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gwdjnfdup.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/ggvkgbbed.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gvtvxiwnj.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gevkqdsly.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gjzgdodjd.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gzcweeiml.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gyojvmvtv.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gbbbocbrw.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/ghhaqhhju.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gqpmzxxlb.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdbfkry.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gwhmsrnbe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gasixahjy.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gezcvirrz.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gjydqccsb.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gryadjdtn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ghdwckzwc.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gravhdswn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gkbxnufqp.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gvjtzmjzq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gtrmmtted.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gfxupxvgk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/goehzqbnq.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gblghxkbc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gsjqctbeo.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gxiedpsrz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/glxemqitf.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gqdfmchgy.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gazrfaxmd.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/glqjkxtez.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gwefxdrrd.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gjqacelit.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtgthsgpx.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gdkyukgqw.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gntqldzqk.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gwfiwqiks.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/ghfkztwwf.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gpdzfnmnr.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gdukptufe.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gfkojwnqb.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gidxhkvcb.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbcywiwmv.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gsjxwptxc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/geydjjdqs.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gdzoymxgi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/ghhftgszx.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gwapjjqri.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gjmbjpqiu.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/glpihgbbu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gtqflhbcn.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gmgiaatnb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdgoppqcx.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gzfknrmzo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfphhaeby.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gkxlezfqu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gmpwforom.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gajysoazy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/ghgvdlues.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvvgxij.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gwoyvclpq.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gqniovgbi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gjfkjhhwv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gtdaeyube.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gpzzlqibp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gxqhzjrtd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gbxbweksd.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gxrnhurne.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gwrbomtzn.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gmqsvwfel.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gscinfskg.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gcdlxfdxv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/glhilovtv.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gefrofnil.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gknzwkalg.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gcphexyhd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gwzlvhcxq.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gfnxwwhdn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gcjbzxigd.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gpguixicc.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gjhujcoyd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gepodltdz.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gvvgbakwu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/grbxaheug.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gbsyesocg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gnrcexacd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/grhlbwhqv.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gulwrpyst.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gzsjsipus.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gxjqbbswz.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gmxixeitl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gvxlqjsfa.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gzrwbtttv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/giqetugrt.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/geknyuosg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gpfmguuxk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gzlfnqkaw.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gcbqpwwct.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gasxswxoj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/galoyamck.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gwfxwgxlk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gxrqorjqv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gqwmnjlhj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gsmufijau.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtyxobjsf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/grribivzi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjkjdldfh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gkvlyefbw.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gahaszlqf.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gphpcdtbg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gaccrgnox.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gepfgyypg.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ghdynpczf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gblfpverv.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gcllrumsu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gvhlfgjfx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gsyotmgps.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gvvfdpywd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gaeooholu.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gbbyqillv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/goaerjbsp.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gzbirqkak.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gkvwrwuva.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gfmncccey.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gkigydrbf.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gunhwtsar.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gqpcriszr.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gjjuyegcs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gvjigoswr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gefvnuizn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/getfldlfc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/ggtdsrctx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gzntfezof.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gqabjcoux.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gundycquv.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gcfqhmcuj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gsaxxxkuv.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdcaaqvdx.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggfljgcsw.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/geczmghss.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gaqchexua.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/glotmfrke.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gheggzxtx.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gbsdimhdp.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gpxycpfgi.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gujzgbydi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzyakenv.sHtML


<!-- 参考信息 -->