代发 wailian999

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjjzrpwk.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpfrmayg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/getqidetd.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gaokkamgx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grqqkvkaa.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjxfavld.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbvqdenb.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmvmsrvg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwywnovcp.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugsthay.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfegoviu.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyohnjoyg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwadctzg.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/glttextoa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxgxtjlv.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghungstwl.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gffuayhpm.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gvfjsgjph.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkjmyktcz.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/getrbqzmx.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmydbfwqf.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnshefexy.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gouwzjkdc.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndanhvfa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjbaipwh.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeusacjn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtstzrbv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/guttannpf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdxxfsfd.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypttpxdh.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gnwftwfjt.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqejmppw.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtulyjhc.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gapudwdca.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnqizsyb.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtfndnmfg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxjxutmjc.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gbzgekzzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gugzmqyjy.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghyarplan.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbakiclb.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/geqhlzncu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjrdjqeq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gglhzytue.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/geqbmadgf.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gdknaiamd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjhpknov.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gjihacats.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcefmrlp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gasyyncik.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaxskcbk.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnenfeejn.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzipovrvy.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gktizoewe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwgivhym.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsjjsxsf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaknebip.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfcqcfix.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgbfwifs.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxzsugux.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbdwnlot.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/ghvmpesvo.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwheauzyb.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsnnndljn.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghixysegm.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gjdplsdrb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqcctvnc.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/grbbsfhpj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gowlkimlu.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfnmyqlq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvihflnis.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhvgqtsr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gztofmzti.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gypvikngy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gequrkpcm.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqgffggvr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffenbyvu.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpnzmwkd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcgexrfy.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gfurnoeud.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/genwhhtvv.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gpuoqanjk.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glkrjokbf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikxhswcs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gciugwkvk.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpcftview.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdsdnywh.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfnvwlue.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gzasybgmh.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzialzgfo.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrytqoev.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgcwsptg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaghdypy.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfmbpvnhm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsecxldq.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaaawrrn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhaqlobp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gurxxinfv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyijkagr.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvcyujhh.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gvhznqsiv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzbovajo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyqubxyq.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gwnmdxaxq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiwcoelk.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvqaqvae.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gvonbqjrh.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/givmgvcuj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gffnqwbgd.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuhnecgq.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gofokfwcl.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ghbcxirhx.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gioqmzmug.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gwrelwyol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnslhuwvb.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzjkfcrd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gclsoqtol.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gfjesrwsw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gknbptjym.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gttjiciah.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gmnnswoko.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvefpiwqn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiuvqguq.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gfbsbqwjq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqqajkje.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwycjzkn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyjecmhl.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqrsxkfyv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gajusejov.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gotwuaddy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/giveuovsk.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/grdshpmij.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcmyizyj.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/glvdkhvrv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gluqegkhs.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gmttvydqw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmyiftar.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gtelthbfc.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gqatdbeaf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqtzqdhsx.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/giyuhdhho.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqylqtezn.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gipkeomgz.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfxquoit.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzynlrbyq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gritmlzfb.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gokdxjxop.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gpvcaxuyb.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gjbsgdzaf.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/guazsadlz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gacsxiqbc.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiboijsc.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexopplkr.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/garkopzph.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gwajhjcif.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gbzertkxf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsqjsldh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxwqhxrw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gfpyksqgu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelbqmzrl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gyttxwsab.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkepdotjz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdzccpdp.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzupvuxlr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gctllened.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghklqtigw.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnhkvhtu.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtexcstnt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklqjmzxv.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbtonkeq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/geejyrdwv.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gfakvfbyn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbnywifq.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gjychlsof.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gecmxrcol.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/grulcrdcz.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gxkzqjpcz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxwzyxxfw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/ghljpnidt.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjderaec.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gclctzvnz.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gethivste.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gmitrgabs.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwszcerxd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfgeylryf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvxpwztc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/grgmutlpu.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/goskcpouy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gyestfspc.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdhkfpzj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhankaks.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnepraai.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxipemgxu.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/guxjkjghv.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeueqlgi.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeafrroo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/glachqjpv.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/guscgyzmg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcionyulm.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgqzdsur.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwduxirph.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgiotvnd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gsiqxaotq.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/ghpfmmece.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdeojnuc.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ghklguowb.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gczhfswlw.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gddkcqkyw.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxdhqeah.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmkmjokc.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/giagqmlti.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gquqbcnuq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnhpqgng.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gthimkwcl.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/givbnvzkq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdghkenot.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoarloom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glmubltht.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/grbyrrsla.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxsodyxc.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbtudedr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbjnyjzo.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtemmbbpf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/garaobodk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbfrkwza.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gyrhkpgar.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgyzrcyp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdohdzoac.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gltutjbld.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/goqdrbmuk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/glwsldawu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gljezeens.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gfbsfhqqz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvidquok.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ghriinaaf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghcwlhooy.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gjjuvctjt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsshffleu.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwgdtrps.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhqkdjsd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/goezkgzas.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqgutapy.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giyxsfdtf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gxixjgxwc.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsavxehc.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsnvuugt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufgevpfb.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gdceurjgh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gqfkrwjku.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnzzxhwu.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gnzdsjyxs.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekebxrjt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geerxtbiz.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gxdqkexlu.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/glqglnlee.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmwtmlai.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwlwebvd.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfrclfiz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocfemhmk.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkmctsoq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsxclryfp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmshnchho.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggowlnizi.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gpygxfekd.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gxcrbwzao.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkakucyr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrpgibkj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gaccodzoh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/grhestxap.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdofjxxe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/goskbsqzo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujafjuuj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gonsimzvt.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmefrnto.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gibcgdxeo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddclgcuk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjnuntph.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrpwalej.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gchchykbo.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/grgnzcigf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcwiliml.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgzcjeq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/giobubixg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gojgmbrmz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gioaadfbx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywfeozxu.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsvkuszg.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gmydizpzv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrncpjku.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtfqbqgm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwgnooim.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gezjnhjpp.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/ghpohhthf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvbwrhsw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gthbqynck.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkeuboerf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/ginndebvx.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfbjmxrqo.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gunvsizdy.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gssxmcusg.sHtML


<!-- 参考信息 -->