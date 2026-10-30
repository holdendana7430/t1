代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gixjstuzl.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gzjtndegv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrujopxn.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjrjzoyke.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpzhwjok.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/guzcmjunm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjulqmlec.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwgsxyaw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdgyyrwia.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gszjspzlf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzrsmftj.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbqundkx.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwehfmhpa.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosmxxjiz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gavbhmdvf.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gfcujmsqo.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvytqenbf.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gjrewpbeo.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbojmryzv.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddcxzour.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpfuhiron.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glyiipasn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxcokcnza.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gyajbajfg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gutbrjxqy.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkzpocps.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxqljqru.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtechcurd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxwefpya.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gjofansny.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/geqqrgwgg.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwtmgysz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqfyterr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamjsfdey.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzajrfcj.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gaaubijjb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspcljft.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gdazdauyi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhwfxnwj.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gvwrhbcwo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxzbgxcb.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gestftbcr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwiotzpti.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/glsroivsp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmichsfcs.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnfogcpp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gubffsiwd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guomwriyo.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdevzlxdm.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gzlhfsyeg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvouzhlb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvhkykwd.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/goutsuvfk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/glcxunqyw.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gcrapbqzs.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaxytigj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gufxtfpfd.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjgngiag.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrcrbfsq.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gewzeadxz.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gkofmkirh.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpvtgmju.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqunkuser.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gcvlyzrdp.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gnouppsvv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givicylud.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwblwwgui.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljvjruxk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuttymsk.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbamzfwd.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grhxlnqms.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genpjaycr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnmftzgd.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gieumxskk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gltkvnqrs.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbvzpjgo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gbjoosjsx.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoljcpyc.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gatvtcich.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gipjxrzfy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhnjmevu.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gorobvpyk.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gikmqrpij.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/grdcxxrbn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gxozjkrtc.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvxhxwql.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gdpryytzc.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfxdtely.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gsjqeqevp.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtjobuil.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gahblemrv.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gyobduspp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhxhixcm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjptwnozx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkmharnt.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gybilgrqj.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gsntfmnth.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxvgirdw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfovhsvch.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/giuejcgki.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/grkudxmty.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gswsmkkaa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqjuhyxr.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkzmkmvl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gnwrydtsq.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdwnpcpk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtphfoeab.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gajkyxege.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/girmgkcqf.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gsudqzrgx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrjzlnmt.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gnjhuzmig.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gplyyaiuh.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gwnjhuysf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltbegnzt.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gohfnpmwq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhjreytv.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/golghwwmt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgeuxzhi.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gwujygwze.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gbwctqxmb.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gdovcwnoh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpelptsvc.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiexzzrq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/geblfnwjp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyjxyfrs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxowbeefe.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrjluqta.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gqflupvvu.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gbufgbenf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoyqxqct.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/ghteiirkx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbwexscod.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcquctna.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsodydgqk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gomsceqkc.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfldzuui.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrkkjaia.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcdsgjoab.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gktmsgrbo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjtokyjiu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gtrwgbruu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gilgrhtjk.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkqtedks.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gewwmiswl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqxtmalc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqgcxiwz.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gccmearzf.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/geeivhapg.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqhyoroed.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqrdsphs.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gsrpziayv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpvgcejd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gafsdeuaw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjigclqqw.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfahtuag.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gvsscqcdp.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvhzpesi.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfoajhun.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gewjwihgc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gxvrmprcw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grfopascu.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvawiegv.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gngkfiync.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gxxdhoaam.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gjkeffnog.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvbudnte.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmrjrmkr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gildtupeg.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbetcvzv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumpynkxv.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrhczsrm.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gboczhlsv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeiujqjb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/ghqzkehvq.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gtgkchhhj.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqxfhfdu.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqmgokmnr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvspgisr.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmnonyrmu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/goowxmckv.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/geknmijyy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmhcimpl.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqtatutx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gemgabslz.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvoamtwt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrwijeim.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gofdxthhw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gomgkfhjc.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gsberserd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gurfqlart.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohyxrqde.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzlfkbrc.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsqmrguh.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnadcprqt.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvynozsc.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gvomawyvg.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gywerdxhx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gomzktivx.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gslghidyh.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ghecjoywn.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gckmuflpn.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glesqsrhq.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjenuhedp.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdcobagh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gghljgtvs.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbzrtgea.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gtboiqjoj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gaicsvjho.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gztysaqdq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/grvpsjuah.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjyychky.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gitwpyhuc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gicpfzktm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxvmnldj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnlqikvul.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gsfblhwit.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjstqdfg.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/grrnqnkfg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjamkhos.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcprjqeqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gtzyytmiz.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkhpqstk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/guxlroiee.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwagstjtp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gbhytwyfe.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxccguljg.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gujpuxben.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzcxvcpf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/ghcighvks.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajysrhux.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcaqfjjxw.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxfiseed.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvxjgedi.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdsvbtyz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugbinhzh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gplhbvywk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtikypvvd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbpdhlxv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gdpadvihp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjukokltk.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqlggmqyn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/guyuhhhxr.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ggwvzldwq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjidguczk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/goutdwkjp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyzcbjwd.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gccrotsye.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpebhyvbp.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gdaxotydp.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/ggcoszzyt.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gslqwmvso.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvhfkhbe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsudhwepq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzchpmnc.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaedfehmu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gujtwlpoh.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyetyrzi.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtounyxma.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ggcilfcwn.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gegpxjxly.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrcswcse.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguupppey.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gancrpwug.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gxmhhtdzv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzeduxwbl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gvejqhszc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbnzodgtg.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcqsqbai.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/giyjwenlq.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/glzuvnbvi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmfifkeu.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gzhwkvqpa.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfnkirsd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gcajnvura.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/guybqoxoy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcolmteq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/ggxqkdxlp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/glwpmrtje.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkcboetnx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/glgfgajjp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/grbnpzfrs.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/ggiwraiaq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gneailwqu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccxbmdsm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurfplutx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteajydzf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gmzjopmpx.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gldmryyqf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gimslujru.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gykhwizer.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/guhdfkgdf.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gfcrfsbqw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtuxrcgzn.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvstmcgp.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglinxlgs.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/glfqayxvu.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gboywhyvb.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdtomdrni.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrwusymi.sHtML


<!-- 参考信息 -->