代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/goavdekwl.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gkaugjjyx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/ghopdzgiw.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gcorghwsa.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gzkzhvoed.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gbqvlkfvy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gdfnrqmro.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gnjgeigch.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gtfclgmhq.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/grktzqhcj.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gofupnpkj.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gpvwtqzzk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gtzshgtgl.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gyapqnqwr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gewloffma.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gihvbjrzg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/geulgzhhi.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gontlclpx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gzsebyzwj.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gfhuppltp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gqhqxuljk.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gucwzizxx.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gvdqzctxo.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/glodtfozp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gekrbnweo.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gmkbuypew.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gofdsncjb.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gamrbxiks.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/ghmzecsuf.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/ggchhleas.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gmvveklpr.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/grykazyde.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gdmsvgfyj.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gwfnoafzq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gdtjjyafs.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gdeoexxtj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/goolfrtgm.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gyfgcsngf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gfimksokd.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gdceoihsy.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gidlqatfl.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gyhfvqicl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gitvkmlkn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/glvioypur.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gajajoqrw.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gwawdnsza.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gpzozqmgc.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gguuhdqvr.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gfhocabnn.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gfwwsdwph.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gzxewzols.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gunhrankd.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gkksvuavv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gguvgstqs.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/grwhnotyn.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gxvgihyyc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gfexmrkpx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/ggmssokez.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gbzybsted.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gqaktwkff.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gcaeuqxrs.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/glliqeyqv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gidfbyjzk.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gqhjnankk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/ghfdwbkwi.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/ggsysnyhv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggfmktqdf.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gjluefddg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gxxjtzzzb.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gmjibuipv.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grhapgxiz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gznjxmemo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/glbsszvwo.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gumwxfdpw.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gmfmyicqw.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/guzntxewu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gsiercbyd.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gskytvvst.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gpyyyhkxa.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/ggwozgzuz.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gdatjtbdv.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gnkiqnmpg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gsgtuaesm.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gzifxkzhc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gjtgprjwd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gxzphcuiz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/glzjdtgwk.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gctmbxfmq.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/ggnvbtjcz.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gwrhbdonp.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gqsjwbwbh.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gjagdwgfo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/guqrbhipn.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/grpaouxxq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gkkescjab.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gkmirwkgp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gnjnmlndf.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gdflmjwgj.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gyheyrxto.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gbipircxc.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gqqtwpeby.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gqbjmizqt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gfzrnpzti.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gomujzees.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/grpzwusws.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gdqzvrjyh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gmzrzevup.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gceewkmrv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/ghffmjdgy.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gtweeqtuc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gvmrxicfu.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gzmfnufic.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/ggedenxlq.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gdipsvvam.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gdaydwmzz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxcvsyzbf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gzbacgqca.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gnyrfkkri.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gdtsiviou.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gvdodidhr.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gotlvnlde.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gujngwlsv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gysfkvjhw.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gpludlxiy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gdzcklkac.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/ggygyezcl.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gdxesmtbr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsmvoerby.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gzxobtyht.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gahbhfxrr.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gidowvbtj.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gwegtmbdw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/glfquyhcf.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/galbfgral.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gdzzslqds.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gxsgqgeyd.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gocydzuvb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gzadszech.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gspolauaw.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gtzndcnsm.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gfsdirlsr.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gqnkewgjz.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gzmkxzfli.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gsudqzchg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gjvpeikng.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gijtqqply.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gbyrwsfgs.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/goyxkwmmo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gglssvxmy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gnpsanerc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gatyecqzg.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gadsrnmpz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gdggsyusr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/govnbnuxj.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gyolbbweu.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gaffxjezx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/glkdiwipz.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gkoyctuoq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gcmzjyusl.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/goskkqzqc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gsrygsiya.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzlhhmlza.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gkgtffmak.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gyzgvexkl.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gjwbrqdcv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gpnrghjov.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gisssvzof.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/guavvqgrh.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gjwtxdjuq.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/genmpgizo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/grzxucecr.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gqjgbmbaz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/grtzjwxpu.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gwxifftnp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gommvmwqe.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/getxylkkj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gglsgmejt.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gbjliaynf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gfutmibtf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gqnsugswy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/glslgoubf.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gigewmwtm.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/ghkqbmbtc.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gubnsbdag.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gwztqxpus.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gqcqjeznu.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpzxzvkes.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gnadpkdrf.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gytbzbelv.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gxyfedbae.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gwiyjwmkj.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gjiahyzfb.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/ghgxuvmby.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gzrqhlgih.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gsbovqgdm.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpgvyvmlp.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/ghocpcmug.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gpfursytj.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gaehpjjcx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gmtooeatj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gemdbzjtl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gczreytnc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gwlpdaueh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gufluksyr.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gamexrtvf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqioliisu.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gdhpyfzde.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/giyoxqfqp.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gsiyguddr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gehwyctku.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gwsswacwe.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gviagqfsw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gjtfjihul.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/grzasqehy.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gwrwikpeh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/ghidtivzs.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gcssaumbb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gotktnqiz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gompazspd.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/goxxyebzv.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gzctczrvh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gllagffgk.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gdfaamyfx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gxjqkictr.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gbbasmrpn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/geylkyogx.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gdqmmhvjt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbhdygzj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gxxhmdcxa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gjjccbdpe.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gxxrlqkew.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/ggxrghvfp.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gjcadancb.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gflfawtci.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gwxfpzuoq.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gkjkccqam.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfoabmdip.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gxgdlzhqk.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gahsptipw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gtbgucqna.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gctzprmqs.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gevedzvsy.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/guesdqang.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gvywpmfnu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gwagugqab.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/grhxzpfjz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gnlaszwsx.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gmfmvlczr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/glijcewew.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gpinmsola.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gzgpluees.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/ghjpvdqrc.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gpwznecwe.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/goiovgowr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gqadbveup.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/ghzarskmk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gqqdvwzgl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqnmsbgvt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gewpgytyd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjohgbyqg.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grwicfery.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gergyprmz.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gpbwupjnc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/guhipivxl.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gzvakwwpx.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gjxmvqkku.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gikkrsrkg.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gjlybgrww.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gzequklyd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/grcglsrsx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gspfmufrn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grpzjqgmk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/ghxkelaar.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gysxxgrul.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/govpniabw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gmampwtiv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gshmnppjt.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gholemblc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gpipfermt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gdzaawkyu.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/ganobvixf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/goelgbage.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gidiexpmd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gqpaccyzi.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gyweyixwj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gcyhrlfqy.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/goecsuede.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gfbwdghzn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/grncxvsnc.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/giqrkriof.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsepkctrm.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gcuiziunv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gsxtqjdoa.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gznysbext.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ggttlfwqm.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gpcjdikor.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/giahiqump.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/ghmpdzsjl.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/grjzkuvlo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gvxidelgd.sHtML


<!-- 参考信息 -->