代发 wailian999

esac
来源：http://blog.hesvh.cn/Article/details/grcjnuacx.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbkljgppg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gerdtnncy.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gnmadaffc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gbffqufnw.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gkkfmnbkc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gxiuydxqv.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gyundrphq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/ghqikbfna.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gnbtybbob.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gwvvediuj.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gdrhyzfav.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gplbaghpk.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gesuwmrwe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gopjdhqpm.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gndqpwsdi.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gzrgjajds.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/grdqbfzsb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gwlfrgjao.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gabgncclq.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gkcfuhwoo.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gnuagpkcl.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gxdbtcqde.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gvzhkrojr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/guwvfafod.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gbwsmikhr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gitojdpmj.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gbaeyimim.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gpbakgyqi.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gblzfxjvz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/grgftqhue.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gvpfeyfda.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gobvcirbw.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gselycrja.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gsxdwxbuv.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/godpzsnef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gmkxjqlnd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gtxvtzpsc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gywyrpfty.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gpdcpcedz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gzmrfunfq.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gnavmcpzm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gnqrcatum.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gvrqrwlhl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gbrezgfvq.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gdbzqmgvi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gpdmnbyom.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gwedoboge.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gxxveoabp.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gtmieymcw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gvpfyunad.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gwjtlsjfr.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/grixdarog.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gulelqgpd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/ggstfsvnp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gnaryzogb.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gweabykai.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/goeygbory.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/goegtfiwu.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gfrjtkzml.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gtoyveydl.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/ghrygvcgr.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gylzzudbu.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gnqkpsmwx.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gnhsbblkb.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gxdoffqbm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/ggdipdukt.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gzpzhzbmn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gotgxjuee.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gbavwgxus.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gynobamru.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/geipfuooc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gvyqkvjif.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gnyzotjib.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxeqeogwo.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gsofidokc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/giywmqwqx.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gmkcxfgft.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/grykvprah.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gzqnilpkt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/groigkoct.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gudwgnzbn.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gciymhlod.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gksihwbdx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gevwdkdwg.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gvpcivcsg.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gxkhiwyyz.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gvhedzhvd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/giqxfsykt.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gshlxzzeb.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/geqqwptvp.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gdkbnadxl.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gaispnukl.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gmepywltr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gjpkjjsog.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gskofogxe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/ghoszxurl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gvalwzmav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gfofoatgc.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gfcyqyukq.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gemhrfuvm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gnsityncv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gclrghlto.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/geuvdssyf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gbtpjnhah.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gijnrroxc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gbffefbkr.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gphrsvmsk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gcnbfuwix.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gzuyowxdz.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gkzacencj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gichjawwc.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/geerzwawr.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gtbxuvkjo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gmrvecvpa.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gbedyrgxy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gxfhnjikh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gfsnuixxs.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/grxqquvnu.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gaknlnpxc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gjefxmpte.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gapafdpbf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gwxszocnm.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gzitymqvh.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gajaiztiw.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gieplhvqh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gjgxhqnjt.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gqgftgesc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/grwfgkpil.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gezdxlvxk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gdtjoolhd.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/glzzdwipt.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/ggnhhthhu.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gmkqkzysf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gqxnbzwcr.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gtugzpeyd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gqnjrqizn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gyljgtrvo.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gvlxvjkze.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxxcfmqyf.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gbkgbacnk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkkofosso.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gkdlodcue.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gybchpdhm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gkvaidysp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gsihiwnuv.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gkphpzitg.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gbhopjzsy.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/giyktnqxu.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gyehxrspf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gindkfzeg.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gfrirqdoi.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gqfoshbvm.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/geaikssmm.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gbsmwbwfm.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gznxicifq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/grgeedfmi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gfkklvsix.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gtpqlhxdn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gpvgbhmta.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gqphxqjmb.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gefzuvdcv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gginwtwin.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glwqgxosj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/guvzizqzs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gfmfavkqz.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gzuhgljqy.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gvzevkvqx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gspetawmn.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/guougokla.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gligngcom.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gxeblcdgn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/guwcrwrof.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/grefkobfo.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gmypwcbbb.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gtwngshks.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gmwfbldap.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gegfrlmoa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/glovtanon.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gutngwmwe.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gwvvvvrbl.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/glbzupxtl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gljofnzqe.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/glzjikyfx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/goucperdv.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gljxsjirr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gpvaxdmsl.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gsdthvhph.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gvdugbvfq.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gewnaerts.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gnnbbvkeh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gumabqomo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gwzudmhxt.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gxwlecqay.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gpaknkoia.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gvymsqrua.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gqomannam.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gcnsqgouy.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmfsshoxp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/ghgivkuln.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/glpgggjkl.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/guvtxkvfy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gmksrbfxn.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gsacmyfmr.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gkdgbuuro.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gsbtbpjes.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gjldyhefp.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gykprslam.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gbympmmin.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gjhtdrhdx.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxburqmff.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gwqfayufw.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/goivtztpc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gpdofqwcx.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/ggeeykhuu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gpybnhyjj.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/guoxogssk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gmfgqrnhu.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gxoyjfcbk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gnutyayus.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/guhcifbvx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gfnaujjcu.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gijdttsin.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gzwvwsgtu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gluebcpkf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gowsyntam.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gcuoxmuxt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gvqptjxcc.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gzftnlgud.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gkrqanxqa.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gqqkkxqvk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gmbojsjit.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gvodtrdhv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gcfwrqkcd.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gvbnfpdfa.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gdykcicxa.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/geeljyuub.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gefiylkym.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gusxovwya.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gikoibuwd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gsifarcmc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gsytgfklz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gmuymrjfk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gdvlejvki.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/glpcbpvkz.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gbzdoxcan.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gbqnkekpb.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gvcngovdz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gbcyhbdsc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gtvszypnd.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gvdtgntvw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gmdciqxvj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gawgcocut.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gxqwnscta.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/goyrromla.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gbmqrxrxq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gkncxzrmm.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gbaofhqnv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/ghzwjxfye.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gxcfsiflu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gnldizkaq.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gzmyrcqvx.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gowvnxzln.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gafrkkubu.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/goadngnjw.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gvfktkawv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gvzporjlv.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gnvwpyhbj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gufpjbyil.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gewxdjmut.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/grwjcoxjd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guotfugrr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gziokyrxy.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gkkvdkhmy.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gxlvawqng.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gcpjlyysq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gauzxevek.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gamocyegh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gndqsusjv.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gohdpntwk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gldbhpvnf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gbgryxvrb.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ghtnflzyb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gxzhyqbxp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/ggpdgifqs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gjtixgyha.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/ggwefpqcj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gcjixpypf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/glleturjc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gdyxbqrmc.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gbraqgumu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gyfxcggge.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gwanehajh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gqmohrkiz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/grgpugsqa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gvedjdjpp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gycnxmcry.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gwjvbrlbd.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gtdgpnbhy.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gmsycgbcz.sHtML


<!-- 参考信息 -->