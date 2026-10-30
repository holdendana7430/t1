代发 wailian999

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gsddwrcgq.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkpxlyog.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geyfeccxh.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpromxnh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkchcbibd.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gfnayubvp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggscnsung.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmylbrsr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjdgshvi.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gopdoenon.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gylenptba.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnlzwuse.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrsxgprg.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gykjwyecb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohhipuvq.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gyoqruxcl.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohtiijmm.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gwxsskqxi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkryryuu.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvdiraem.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gumoihzdx.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdcjrpvf.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/grqyzysls.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzsdzcljf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcktwjeje.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpzxbnmhj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfilwgpy.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gugyyuxon.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvbufwsn.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvchflekx.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxcqhmca.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gioepoopj.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/guhhlbuwf.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/ghexwzivi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbudrizlo.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/geyvknygh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmavzeyvy.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfgvirc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gzuqrovxg.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpijdmnu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gujfwsweu.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/goiwhnhos.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwtdgqpgz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gkasxisxn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/geqocscfi.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gpybovoxt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwmkurwu.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gsqixkouo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmleourku.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gedcizkwl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gntfctmag.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvhjoqaos.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/geihkllmg.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gdsqiaqxx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohfuxlsr.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/ggojccuaj.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gafqwxmvg.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulwpzswo.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gfevsoohn.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbczjzlc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gldofiizh.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/ghxwqwlps.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gojkbyopo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwotdlvd.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gyjuchijh.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdhgrasq.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gimnebhdo.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gmzrlmmbk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwlmpkim.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gyxtdnmdt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gscttwczt.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghsgmnzlp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyncmjtm.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gkaoyybgu.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxbwwatrt.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqhgmawwf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gihjhvoeb.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gydhqeawp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guwwhqgfo.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/guaonpolq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtjhyjmw.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gyexnvwla.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkivsxaxk.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkxzbgwk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpkogpif.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzimfyhh.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqmegdyb.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/goaqytzmm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gshxniqxo.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouobvcbl.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/glatrmxkn.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gxcsmjqtz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynnwfbdt.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gppaqdjqe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgaqosvj.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfnxbrnz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ghstyrmkh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkxzyxcw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjrfiayo.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzkmvzy.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gvdqnqhim.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gctugceez.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gmqwmmasm.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gtlsshsob.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/guilckvfp.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gzaiidbrx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gawklhknz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbcqdjah.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gfskbwuys.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkmkfyjx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlsufltr.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/garcmshnk.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdysxjtef.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjtfvhpv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goykajjqo.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqnuixfv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gahyjpnvm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfmfogjh.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/grqtxvgdw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfizohdt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyieefxav.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpzgzzal.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gapxxybcs.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtcueyqex.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/goikkkxma.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gzucdoldu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwridfvj.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbauksvdq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvpzsdcf.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdtxnoqhu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gluaufvte.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/geekwjjnh.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gahutbfus.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gdarrqevk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glmaayagv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcteonenv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyqjwwzp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqsyfcah.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxlhohps.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghjdghwjn.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqiuazwv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goplhnklz.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfzgtekta.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihdwztkf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grneteunh.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorkpqrql.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjeynvkvs.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvgomuqx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnzxjowv.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gtandoqkz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtcywarz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxfzpaps.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gofycagtg.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grnyuikpu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrncvdne.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgimjyfw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gjlbkphju.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/grxsnvoun.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gyxgnvsxu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdashugqy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaptfgol.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjbsthpu.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/givkomwzk.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaovfxpor.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gjlgrdbqm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gitvvgeif.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ggbnhxlju.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdhqaysap.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ggjbfkdmg.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/grjzsldls.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvnzxiiq.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gyamafdab.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxydjswz.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grokwmgjn.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gxlbqhbig.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gyxtwldgn.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/getnfaems.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmklzbfm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gadwvdbnz.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpkeikkyz.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gpngxeoqm.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrffzbyn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiosyvzp.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/goyezpeld.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbvvruuz.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gsczsuzxp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/glnhoyakk.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gmewwdukp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/glhuzztuc.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/grxctqduj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfrdscjs.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngglzmq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbktwqdov.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbsvszcs.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gproxpvmn.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gdniziypv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glilgkzfj.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/glmyxiwxs.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxngtkyxk.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxyaeyrj.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gjbfecajm.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyyoeikc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxlkfjrq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqteqkid.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gwygxjyom.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqgolzihw.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtgxkebg.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjnoyoutp.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gvbolnnnt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gujvsruye.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdgtjlxi.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gkipmatyr.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpnycbxi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzswsxzh.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gexbwgino.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gclekeyij.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxcdnkem.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glmgwkugy.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/grvpywufu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiwixhav.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/guqdbumug.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiyydpgr.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glxljetrd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdjizkyl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmdshwnc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsmqwydv.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbewqknuf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeofhemk.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzfclxicy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhrpsmlp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvujoibb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gpzsehmuj.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxurdrlsf.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvsngezu.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/glecixscc.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxafumlre.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gyngbtdnz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjitjxvxu.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gccsfhlzg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gewsyonnc.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gyevtslin.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghjjzdgvx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glebtzpxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gqlvjbtgu.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdkygdyzl.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcxjmnfnj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggimavkao.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/giqmnflco.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpujxwqjg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/giaodmggt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnubwfjx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcyuhecz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/glwlzhlqn.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkkktbnm.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gsgdtgekh.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goypgjbrm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gchjlimoe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibpzchpf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqthuzngr.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbzvihdj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjylnzfuf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscgfauoq.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaescmsvd.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvucanei.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gipspktay.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gejpnldrc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbnpkysu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gtpaenhoi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gifzzbsac.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkcnrnkt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/glihvphiu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtbmtfupy.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfmlmzcr.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gdzwwpwcr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvnknawc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/guugeiodj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaidvqhjc.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gkemdtdwp.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhiwfybg.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbqmxptj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gbitvfwko.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/ghzmtrjig.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gtrqfeedv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/grixfkbmk.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gmwtgxzls.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjkncddw.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ghujzgzcx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gscgdbndb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnkwtezp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwfvkfog.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxsudpmuy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfslldpc.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwcarwqd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/glqmlvxxi.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnazxqne.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gomlihacz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbnqkrzd.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxivfihor.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwwcwgpi.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidvczxag.sHtML


<!-- 参考信息 -->