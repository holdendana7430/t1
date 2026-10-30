代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghaprxkwa.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/grdbhctye.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkppxeuxs.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gudybvuln.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbupvamse.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpdjxnza.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmisvwce.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwcchluo.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmswgektm.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqrxtwxt.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnktgqgh.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkretks.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxlqovve.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwrplvqv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gthijzqvj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gwkdkmsnh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulxneycx.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfsvauffm.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gfobppsbw.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsycouxv.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsplxmzkm.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvubvoef.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gaahjcrfs.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guduaoipo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzsczljfl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcmztvew.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/geqnobcze.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggvahsnez.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guxnhjjnm.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gqimyfyog.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsympwnsp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gubmceluy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqoknhfsk.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gjilleiuz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotzthbir.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/giizoiggx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzxiolef.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjqhgwmmc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheyyovtz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndhatkhj.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gndfgkrxr.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gazkhyxok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrxaqyeu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdijxnr.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gldxygmjd.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjctueod.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbqaoddh.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxgdmugz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniycfrko.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymogoepi.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkqnrpsa.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqblvzpbo.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiislwzb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfzxbfyd.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpjmjeqc.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gpgqoyzua.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gnjyzyedv.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/getfnkgzo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gscdalttg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuvixvfc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyczjpace.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gpjjepugb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvkvjcdo.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoqpclki.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhqahqjw.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajowxiqm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdrsponym.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaebybwa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumwqrbeb.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwlxajwt.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gctvdhvuo.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gvltttelk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpzdxbgk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvrqzqac.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gscrdusaz.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfcobgpk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gxoxbfvwm.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ginxjqnwp.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gptstzhzn.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqnptxou.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsxmwthr.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcenmeoa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gxfjkylch.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/govdubiqs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzerkazd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gsjcjacxa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gwblmnsac.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfwifphs.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gkrgnvplq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwnwipqll.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpptzhoqu.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghefdvyvr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glplgimze.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeudynkt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxitwppsq.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkvnodip.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcbellyq.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gvixjttgc.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gkcflsrbv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/glizktoyq.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gokfxugfx.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiwvigwh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdncgsktv.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gpbvnuyti.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwkuqnvh.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gautxnbhm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/grefdcvxr.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/giuctxaei.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gouwtcreg.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/ggotypuzw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrmavfaz.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gycyshdzg.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvgifujn.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gfashntps.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdntyiby.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgffscbo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbresnkbg.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtvqqjdbt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gracaowps.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/glacxzwpw.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gucvrsikd.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gjnemmrve.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtyezsvyl.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpzmpbrt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzuavigr.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gwzojarqt.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gprbnjkyz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsvdqbyv.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmgvgmdx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfrbaissi.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpoazwtka.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuaaqggc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gynxhbyrv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmusrgxeh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gydjodvca.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gkggelsxn.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczyaytxp.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkfbkapw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/grfbhwfwz.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzywkhle.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibesjrrv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnupuhno.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gihkurmny.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzjlxbej.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gosdjppwm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gdeoddcch.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/grschvwpm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gbbxvjruz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gtppwxspu.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gprogbxdb.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/goiceeltb.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghvcfjrqb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gkmknywjw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gwbomyshz.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqftmrwul.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/graveetth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmwpahmz.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/goyepobhp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gzeazdapu.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpridrxfl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgarrxds.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxbxihvi.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkhitkfh.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzyxjpvu.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzedecdhi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gaszfpyyj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gydqbezgj.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzrhthth.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzalgdtw.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gpjgptuwg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gkrmbhgdn.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwzzekpi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/guajascxe.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gefeczdqg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/goftdhydh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwixuonz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzdkqznz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gxtpjxhem.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gxmxybgxx.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gywrrwdaf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkumdzoel.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gowitencl.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/goxlelsuo.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdkfsyvc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gipojevro.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwpkgfng.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gwcgqvbfo.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqmpuzkkj.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmmlgpbb.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpyaroapz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gyquzbevh.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/guickvckv.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtvgzohda.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/golusjjad.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/grrthfflk.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlwqrrjt.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gdxnlwujg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gigkaizlq.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbofkcaiy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gvqejgngp.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkbrgjar.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfortzyd.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gylmhvrkn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxnneeodk.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsfinamt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmfhegus.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gfzohzelt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gazsipzbs.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqmtevty.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghzznuqol.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/githucpce.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gugrrquij.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtgzvenl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwopliic.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghnkoqbll.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gndpstmkt.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxsfyret.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfpanmklm.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcnlalbw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gxrnlgsoa.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiilewel.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gdmxjnhoo.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gdhaxzfxb.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geqnzxdzv.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuvfhpvr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gagteckou.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gthsvplnf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geaqfcguo.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ghtpozvmy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtqzmcbdf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjczotxf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gjhqjajka.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcgnsqwd.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagsgvecq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gpxnygyqy.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gpverricw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmenndcb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gblsbzifr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkywfefd.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gksxayvbr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghhjwxwqu.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gcqevvtoa.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/glaoavyyo.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/glraqoqeg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gymgwkcpa.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/guxuczndf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaikczvve.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gkyoppgvy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzpasvkjv.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmgeicpx.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyvphosl.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbberyqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gogltkzxg.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gpiigcwyu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrctavxh.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gwytxnxto.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/geeqkywan.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gphkxamwc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbntjhwa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnbprecuj.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxvbdcwa.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gtvkkgpvf.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurksfavh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbeajxfd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/guwgenzow.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gghwzjrwy.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuzxtaoz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwrmoprw.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/glpzbjhij.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqpllnzg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcbyvxpx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqgfqidd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gdvueklvj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gfcfqiwph.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gifrjuzmo.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gfvzcqypa.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqhylshk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/ghuieqbfl.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gotqsqazo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gjtyczclh.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gapnuxiat.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgzbnora.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gsrrugrbp.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmtavyeue.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gygpvuaqn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkzjffbw.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gyyrohded.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gxmprfqnp.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwycdmcc.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gurhahylw.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnnldypc.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gmtqprtat.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gndzfyyni.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyijjusa.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/grfacznri.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gqownkbbv.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gymtpkozu.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakivnjkz.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/ghywuaosw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gueysfjbu.sHtML


<!-- 参考信息 -->