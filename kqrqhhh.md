代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaijfsnqn.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grfqscwdd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/geknjnnhv.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbwgkiwn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfabbsnuu.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmwqrhqd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxizvavam.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlhdjblz.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsqpgfgi.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpkcorkz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmcablxhb.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfxboiaw.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdrwabdb.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzenxsagz.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehlknpag.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gudolpfoa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaodehiq.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghjbhvfxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzuxbrhik.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrpugdqg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmwaofpd.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoiuakqc.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmprixova.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldybesda.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoaxnntl.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooekszju.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gfngllbee.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosuxailw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/grfgxpphf.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gpqvkxvru.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxsxcqhj.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvhddtzr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goovswnvh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvblmpie.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqkmqtpgz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyhwfkrf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpfuzhag.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaxhqjrx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnzuiklx.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gjalhvvpt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdiicjmc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxbxtmhc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgisfhjx.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gaajjjbwa.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghnjsrtgv.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkougvubb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhlxyuex.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gyohkrgsa.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/grmmzpkbe.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzredhuib.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gejhgkvzq.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gltrsmvjj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gntfijcez.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gdwcbpmac.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfvpazsd.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbubibbmw.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gojftrpvt.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gcjjumtzi.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/geqypexhh.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzfvtsuc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuflvqrf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtelkcwcf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gblmlxega.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtochiqsd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grsrlogbp.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/glslxdxgj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqcwjkbl.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggizqknfp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzediagm.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmzuugzz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdujmuvs.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlagjzed.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/ggzsthdnt.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggosduwnc.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpkubgox.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gkrkgwxcy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/glezubsdp.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqtbpnos.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gchtklfwa.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfptxspj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvegpkra.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gbrldtcre.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gtolioxog.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhcoejpz.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gidxvldjd.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmczzxxjx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzsvaggb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/grjsnhzrm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gunqyogij.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtrlupgks.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gyucecmac.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfqmbrkr.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gcnnutknp.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvlxjjoce.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gugtkwfcj.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsohuqhe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtduijrzs.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gqufwnelk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpkgucmx.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmglrzxfp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gaognahjx.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gckfawpld.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gipcofqzx.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvhxvatk.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtnnlibz.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqgcqdqw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjehbxwna.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gszucectd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihxlxcas.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gasfrguno.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/ginkthtso.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gpmxpusia.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/glapsscyz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqkrgcsb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwaefjtv.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gcugxoohk.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/ganunrxec.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gbxabtekx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gztfigsph.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/girfuldmz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjssanubk.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsfcikkdl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvkwrgpp.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbuvifbi.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/glxeaidky.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gkezxcwgl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnizaunjq.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/glrrvybkw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjjlsfdjk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/ggpeawsug.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gyctixbvo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gysysfwwe.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gdncaexbi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/graibvmxm.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gruzuitjx.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyzpkqhs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvhmcumqv.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gsypzrnii.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gfbcxcdzk.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gphecastb.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtauhvxgr.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgktnohj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcgtksoz.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkzzctsx.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoaoucml.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/guvfiphgn.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gwonkjkgh.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/glbhqyazk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/girrmzqgx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgmvxmph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gfibxhtbt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbyaohzp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gibtefxhr.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gocezxsrr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfscujsq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmamhdqqx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfvbuisx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnymfsjtw.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgdugzgd.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gztgexerw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdreevdg.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcdtnpjl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gaapxtiro.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcsfhnsb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/goqkwgpaf.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/glzlmjaro.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmkkgndq.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxmkplbt.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/geuogozfa.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmxwxtda.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdevixnwg.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghmecucsb.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfworcgw.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/grohqeaxi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkykhneiv.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gnipusxjc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gohbxrnsn.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxcjmpau.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqywczjuw.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrlvkgmd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxxnbepj.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gctmiyxuo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctljubov.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gwthgijoy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gqdapyhdx.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gppkcvqws.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchfyhyk.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwtbzjql.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/goirpnulx.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gtrnzllfo.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtliigwrh.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gerlwtzvc.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgbadkeu.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/guqkqltsg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbevjylt.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/ggrgbzgzt.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjbwvyou.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyxcfawc.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gcnwqovns.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblnngqqu.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gngccvbgo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiluxhvo.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gatmuixoz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqgvwmkj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwaoxuxl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grjiuvqnb.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpifxxmco.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goymziirf.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gmjhdylqa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagrrknv.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gboffgyia.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnefulmwj.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjeaypvs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gackydjmy.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gqfyckmoc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gztnpfxcw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypvmiplt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosjhlzvq.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gyjvekkey.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwljsobcc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkxybhnv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gswnhgrqt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gppzsphad.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfrmdwer.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtetwwlx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvqdoevy.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gumtmzfvz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqdpqfnyp.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmgelgxj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glvtrdwrq.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gdttbxyyi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gncnwhmhe.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gsldvkwli.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgwtcjvy.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdvfyjsug.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gbxszddzx.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gicprpgis.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmqvepev.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gcuepaisl.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gubnhsmki.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmzfarfor.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqarmyemi.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/glpjwjxzh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gelskqqzi.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdvtwwuu.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gosjkcfli.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwilovafx.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gqausmwtt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gdywnhegw.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gkdyawpqb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokijvrki.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gvkjivewp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcjprzkc.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gpqxkyvxr.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/glansghvf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbftatpeg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwipufgra.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvrzokrc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gohmrtflf.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxcwdxdy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gulfuycey.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvnaqeyes.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gncwvafkm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gflrewchq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghcyjduaf.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gbkuprsus.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gisdqgzsj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpxyqddx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gtasraobo.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gejgxnjmh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gengmnvyd.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gzzludkdf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gnabuzxio.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gavikdngd.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkrupiav.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaanwhnni.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/glqksrgih.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gtqvxjyqb.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfdkobga.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmvzqrtu.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtvkgqoq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlqxvoid.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpxcdgfwr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gcczlcsyr.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/guixxmvad.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqfbglio.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/ggnppjabo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnvqrceqp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrgxtaqr.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gihbllxmk.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhyghcdk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geojihbma.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfrwwmyb.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnfjtlhb.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbhdymdmv.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gciatfhmr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gesfnhbcb.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjnjldjo.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gyzhwspem.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gaknmzdth.sHtML


<!-- 参考信息 -->