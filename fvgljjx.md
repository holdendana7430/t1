代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhqwnyqm.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gekaqqfiu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgydkvbl.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gyfrterib.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfgzbpr.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/glegvllng.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdrbvnypb.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbjuzbyd.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkautpskn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiyzicns.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gglvrxxww.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfazzebfe.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkscyoefn.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gshhvzmko.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjiaypgk.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gygsdzglh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfxqhffti.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gojmvolzp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/geokjllxu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gadbrhksj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwqrgshz.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/glzjzqnps.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gptjzysxo.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gjaxueddj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdtzoqbw.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthyzushz.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/geokttmqm.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpjdpgja.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkjhaxdn.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gufqupfwn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gnbsiwqgy.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoljfbxo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyutjmekb.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorioumjc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgitqeju.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gufqhjiqh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gckwisyxv.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gsnkepach.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gycubhost.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpqkfksq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/goediswej.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsbplrcz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gieqhefux.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjywuygde.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwoqulveq.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/guoyusapl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gutyittst.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gjepazqrd.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gigotzelq.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcwoylmb.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmwvquvn.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gyctyjpdy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gkyqoavbq.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/guqagrtoc.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwmdxihnn.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gubagtaal.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxgctseq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsezcaerj.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gkpspcniu.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnveeinr.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gzrczkwws.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gwyepkeyd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/guyuvhjrj.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnbfiytv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyolkcteh.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gyotefwym.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkteothll.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gipdisipb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeyvrjai.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/geyuxzpqs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxiowivm.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gmsowvmhu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gxtzcsonf.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gbupgpied.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gchonweab.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvosflh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfarktsco.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmrikvzs.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnvdimveb.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ggokndqwi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyvfixvn.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfinkasj.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gatwvdzdk.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfoiflot.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gbukzffsr.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/govpqnxlq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpxmanrm.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gakmpilyc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/givscmgua.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gjxmkgwhf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/greswtqbl.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/grhujpgyb.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gsavhsgzo.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghovewxft.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gljmyvgwf.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmddaqqmk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiokgudi.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdbzrymt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gjlhkvvif.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/glfuktbif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmlqqshi.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gucaavjiz.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvabxcbdj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gobbzwjyu.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/ggqbdtclf.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gufbgrixk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/genzxwlfk.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/goqthvslt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdxoyijz.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gftngzdlw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gghbdlbew.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gbgedvric.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gdmzckdoi.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/glysjeziq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdrjjmdes.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/guvsuzwbq.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgblenox.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkqxzekh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gktbwckao.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmpyclbxe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggakzqogk.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsagjjkak.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ghhcldqjd.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gxwszhjdj.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmairwvf.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gploalvse.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvssnxhiv.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/guiqanbgz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzyfisvv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnbhxpos.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkedwccar.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmedjsywf.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeaudbgs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grrweatbg.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxorihhul.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gvcbsybpg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoikjgnw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxiswcfb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gxocdbvjl.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geawpzrrn.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzpzoluz.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghribcugp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedqvalsm.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gktrgkbcq.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwokmmqj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkhgmqwt.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gaasojqvu.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnchrnfx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjusepevk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gipiurtsk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gjgqorhcc.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyamywxw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gsyeaqjvt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmuzkvtv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gjnlvkudu.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnwzihtjj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/guyjnpdtd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhyfliuf.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmpiokot.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkbbbmijq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gfruveutf.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/grwxkwoiz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzssfkrp.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcuoolmh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjfnlbsz.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvyhmrwx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/guxsyjxkg.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gdbtknibh.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gajntoybw.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gklozifzi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/griosynih.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxmvrkcmx.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsvvizjo.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grggfgfey.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ghprhxklm.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkjizkwp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyujiktte.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcjalxmb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gesorcxkv.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqwnujjif.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/grlmugnio.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbnybuvj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiwzlyjn.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpxmgyms.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglfrnyvz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxhwkmwy.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gvuxdybcv.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gmksgsphq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssicvuvs.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcibnoat.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkcilmzi.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghivgbjiz.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuknbalu.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkaatpvn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmyatshz.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gntnttpzu.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtszrzoo.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpshahoo.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvavnwhgt.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glwjhjiip.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gstksxojn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geoioybhe.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gwslczffq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gqdnfuvwo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftjamudx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/geihksckg.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowdzflyf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzxjflhdb.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gychuzuzx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdyinle.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gvelltqeq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveeerubj.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsfqppin.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grevwvftr.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gclgdsbug.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghexojrdx.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gunjyablf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuwvjgsc.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gueyofsrq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/guowrloep.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/glhbpmxhl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbebspzo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghgpjwfql.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqncvvhd.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gucrfewgl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gqoxthxjw.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqnqdgno.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/glsypngko.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/glvxgjrrn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaueaslk.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gepdhpqdo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfexuhsyd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gfgaxvixw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwxwicgx.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzhsctkxb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/glocugaih.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttuwhdzf.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcviuyseg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxfdhwtx.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gqpykqain.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gpnznneli.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcdpmtkz.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gdewufxyg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxliopex.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjqpnmndt.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gqoasfcet.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepaiqixk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrvzdgaz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gblnbmsmz.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/geuravccp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqutmsymk.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gregkikrm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggasfeonk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvmzlopy.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvznlcpjp.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gtimixigp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwzpqhdk.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gnobxdiii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/glaxhhbos.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzwimplyw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gmidcadbw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guicktytq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiptgoxn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdstohbsc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiyshbxd.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gygjwwxyg.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gltzjeado.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/ghlcorujo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvopspmrv.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/genizhkgi.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/grlktdqxf.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gyfiqfrhz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/glspmljqm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gwwyzgvze.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gjsvvvkqk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gykvkzhkz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxhbalrl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpabfrtu.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gslhkgcvz.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdwtoldt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwtuguhm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/ggzzdjsjy.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdikzbbsu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gabtslppr.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwxpbznj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvybnbet.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/glzorcerp.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gzbfiwcqo.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gbyesivxz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/garhprerv.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gprburgtg.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gqwadlpjn.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbwiwize.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gbclxcujz.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gttmssduo.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gloybodzn.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/grzgrvsbe.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxdzknis.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/grfglpslr.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gytddefgx.sHtML


<!-- 参考信息 -->