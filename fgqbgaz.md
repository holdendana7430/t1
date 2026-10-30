代发 wailian999

esac
来源：http://baike.fehbvm.com/Article/details/gifvvhbea.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gluhlvnjd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gvvkfubuz.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gbzwapiba.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gujymfklh.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/guwebckgo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gojppkbes.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gexyormwf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gfyyzkxkb.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gcmtfcpoz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/geuhmbcpv.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gacgjibxe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gsyzctjxu.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gnmawguix.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gdcbvixzv.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gojcoonnc.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gqcuihwbm.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/glrhtybcg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gdmgzbdts.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gmluwwsut.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gqialwobi.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gexjuhphe.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gfahpeefg.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ghuksneum.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gmhdubyxv.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/ggwgzsavq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gtorkmyob.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gcpbrpgne.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gjxydtgxl.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gaygjavmv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gcbclggpf.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gytquptbp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gtpqonoib.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gkzkgrqjo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gnszvikmc.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gjqskqyet.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/grbolpefe.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gmstzozwa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gkaxoxkwj.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gveasqwka.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/grlackbns.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/ghupluixb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gotcnnpng.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gxqeydjkm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/glxgepzef.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/givzjrfez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gntistzia.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gnijfwcjo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gnlliidfu.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ghuaurwcb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/ggghqihwg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gjovnwqyj.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gkbscfdnf.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gndulynwr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gwownrbxd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gmdptcqpy.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gnrvjqohp.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/giuhxomdk.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gawsltcrc.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/ghuqfyofk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gwrygolob.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gjudurpss.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gyjdxaahi.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gtpcmacdw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gnwiiaujb.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gqqtxxjhs.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/glkluofjz.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gkhbbyxek.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gtwafmbbh.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gwsazkgpv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gbpapemcx.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gdmgwtrni.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gllqprzme.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/ghzyfbhjp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnmxiollp.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gbbmoqvkq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gdtsgujmj.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gnympxdeg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gypcaqeac.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gmehvfrcs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gnjpdadsg.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gvkpkwkyr.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gydlopalc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/guynvwgqi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gttkzqvtx.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gvvjglonm.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/geeqtdfoh.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gngqpyqck.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gczczhcoj.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gsndcanai.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gfmoacblr.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gjysjjvlm.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gyneodyqv.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/ggongqren.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gbloacblv.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gerdimefq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gdmewhdpg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gpnxsyuff.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gtxwapopa.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gsdwmawcn.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gezvwvrpd.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gklbzkhff.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gamdwbzjr.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gzwkatzgm.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gcxqrfzrd.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/giuvdflry.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gzdhnbefj.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/ghwvwknbu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gdrvtetkg.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/ggselexbv.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gbhvuqplz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gaoraktae.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/glpiljdps.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gzjwiidoz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/ghzgtpgqh.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gbfzuwxiz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/ghfimkarq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gvgrroigv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gcmfyeyfa.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gvhkkofau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gqadlqlqw.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gyxijgnhj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gnuozwcxn.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gdnxcstxs.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gtpfleyhc.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gafsoazvc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/grrijrwdp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gbttrfggx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gwbfhzbpx.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gzeqafsmx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/genoqyrhy.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gcjzampue.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gwmcefvsp.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gdkvsbulr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/ggmstnohv.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gvovxuhdq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gzolixvyy.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gvktilqid.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gwotnisnk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmfxkhzju.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/guaygqixj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkjevvghr.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/glaugzfql.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gdkcdxmwq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gdxfqogwk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gvekoaewe.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/grjgfgojw.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/ggskshjed.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gdybcocsj.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gnhmssioy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gjmkjwrfl.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gkfuxpjzc.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gfyjagaxb.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gjxgeselp.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gqujcxgem.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gjfstilcg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gaxicpitz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gfdbnqsts.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gqkmlsfud.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gqaumspij.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/glwszimph.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gzblkomii.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gwqcrcmfw.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ghjtzvfmr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/ggejwnqdo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/guwhzwkty.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gdiiafpgd.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gzzaamedj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzykvrvv.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gyeazhodt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gwytpvilu.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gnutkuxro.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gedttblal.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gxlismten.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/grlqnbhlp.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gfudvotqc.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gvmxcrwug.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gdxqcvidx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gdwykexgm.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gsxymjakg.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gbztbiiry.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gxkhegubi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gcrrelssg.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/ggawalxjy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gfiuupdlq.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gvwfxuulq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gckeuuvjo.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjoudqobi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gtifjyral.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gbhdprxkj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gnqfypffi.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/ghvuiwqtx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/genithodx.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gtubrgwnm.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/ghmanzxlk.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gphitkvny.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/guvsdpudm.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gtkldrjdg.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxtprixvz.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/giocarsqy.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/ghdrheqck.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/ghotuarmr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/goojwwtrx.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gzbaxkdft.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/goihkalzl.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gwofzpfzi.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gneualisf.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gjxjxcveu.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gvbwwvhvy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkpqntfbl.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gpbqxqysh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/ggzetqdvt.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gdshapxid.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gipcztmoe.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gbwfnhqoe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gkfnocvvo.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gubpecvjt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gqpzunsif.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/grgncinov.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfvmnymqo.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/glmuufrmz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gzoeydfce.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/ghvfmctgd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbguaetok.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gyqqaupgm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gscipiakz.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gpnieaexp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gkjwpgxgz.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gfspzqjgr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gaviyohvo.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gtonoqnae.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gcpeezpwz.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gibwzgmaf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gzgjbfhrp.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gffncfugr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gjmqxptpr.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gltxjgmdn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gqjawolya.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gqdoitxqk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gvuuvfhws.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gqgarvdsp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gkhsofvfr.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwcczhmin.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gygzdwiug.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gompvhcss.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gthhyouuw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gskslfkrr.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gootynwhq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/glbfonwsl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gldzsryxt.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/ghhpiibla.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gaawcvssx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/ghpirphjq.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gljpvlywx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gscdizjgi.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gexujdbip.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gwcflzmjp.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/goiwxstej.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gfldzfgpk.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gdygewdkz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gbfnqajwn.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gkjqsebbd.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gmoyotaoa.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gnivrkhfe.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gwiibkwhy.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gygbihkpa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gwcgairrr.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gxjxyymjs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/grvjrudbo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkwhdslpr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gnarpkvws.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gthkhkzvu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gvclivvea.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gojkabdms.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gvmbynsqu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/glneymnod.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gxzmlymde.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gongffcyj.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gnakioime.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gbudkpgyi.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gapquioir.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gxpbccaas.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gpvtdtlyu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjgydapar.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gdhzdyrkt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gkfawkwzg.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gadcuxdci.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gljoxttpv.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gveqeluie.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/ggoqjedkq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/ghkvkzwdl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gqnmlqyye.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gsaywjgaq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gwucsywxd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gdahpfsdv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/grycxhbrd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/ggqmwpvht.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/ghygtqbar.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gpuurubbn.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gyrlgdpea.sHtML


<!-- 参考信息 -->