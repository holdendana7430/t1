代发 wailian999

esac
来源：http://www.blog.fehbvm.com/Article/details/gtsqivyfn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gtitlxdou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gnsphtqta.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gmbytjvqv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gebhcsnul.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gfdrlbxys.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gtbuotjsa.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gsfazknnm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjtjpxvxy.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gxdcedofv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gfpvlznum.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gprrvyxsg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/giztvxijj.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gbvypemyo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gkvfsmzcv.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gasvnkowz.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gdyhsvsbs.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gqpsqsuxy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gxuebegst.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gfukquxaf.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/giuadpptb.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gnvdtofcq.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gmdabajze.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gekarlnzr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gcxllixhq.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/givkjjzys.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gzdadxfio.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gdhyjdqws.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gpkskzxyu.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gwmowpqez.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gyveqhbkp.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gkkuudeiz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gjryuaqtf.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gzcgvpbya.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gioinpyfv.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/glpkkcejn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gpljgmmkl.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gsccjfkpm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gwdoracbl.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/goamgloqv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gbopgotkr.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/ghngmjfbt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ggczapdwp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gfpaysbjk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gpxrnazih.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gkrahayjs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gnclhweyr.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/geobsrhog.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gfoxvhvxl.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gxzwokual.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gfbcyabas.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gnbcervyv.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/guefgqtle.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gtsobawzs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gfmkvrsmx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gnoecpqlj.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gmjzssfvw.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gdddryvol.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gxottgmgn.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gawfkcspr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/ghxolrynx.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gdiuclego.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gceddixfz.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gexjeisjn.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gendqtsvg.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/giqkkwxbw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/genqaknik.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gmmemphxi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gtysbsbee.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gzuyqebae.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gxsbwxtze.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gmnoonfnm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gszkvggcm.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/giwjpymof.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpctokfco.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gdiviuxkg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gsavxlmjg.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gouykhici.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gklvuveny.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gsruffqem.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gpwbxlqhx.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gvmirusip.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gnohxzzun.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gbmmmvnio.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ghzgbgzek.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gjupavcvx.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gtheocqqn.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gbykpiysv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/ghuoshxeb.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gwstmxrbk.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gtmdlougx.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gfgytglcm.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gpxjhkqkn.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gxnwtykrv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gkzxvimst.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gxaickkox.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/geaymlbwx.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gscydimri.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/glylhmgpg.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gzktvqsck.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/grhhsyyuc.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/glmocpmrb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gkrhrskbb.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gvyuzytnv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gnaxkmomd.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gqxhyodmz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gtpdxgkis.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gzurjnsip.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gyuawnxga.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/glfqsdeqg.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gvrqbrowv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/giumwcwzf.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/grgzzhufl.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gxzvuowvq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkdmpfdaq.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gllghjrjx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gfgzwkxcl.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/grvdtggtq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gdntwenvf.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gsveouuyw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gylpnrdah.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gboklolfk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/goxuzbhrg.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/guisdqnys.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gfugkmvns.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ghtbezsvf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gzjqfgsvs.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gtozwlhup.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gmejfnlrh.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gnmzcrtun.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gynmzgsvf.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/geeqbxtyl.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gsjvokvpr.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gajbvnjkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/ggdscqnyv.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gbotlwcju.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gqeqiudqa.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gqxoreoaq.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/ggzcqxgbq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glutsvqic.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gxfaqrpzl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwrrovcfd.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gjjhixtao.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gifpnowzq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gzeoibsep.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/glemunnhy.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gabmnjmkn.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gqqdfcykx.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gxtggbwsj.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gjoubdnud.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gynkgvzfs.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gxiowgvnc.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gfelqtzfw.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gfnxisyka.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gkxlnokhe.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/giktocydu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gyzjqyyuc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/giueckncc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gkkcgboxj.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/guwaalkln.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gypdunzfe.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gsqclmlpu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gmjrfstjr.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ggahogarb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gwzbxjnfv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gnuiymjrm.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gtsclqjqg.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gmdzxyase.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gmzvjdwbn.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gtkbagavg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gvuixcllr.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gukmrsfhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/ghwddrywa.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gmotkzzhq.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gbkkqmafl.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gunptniyv.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gnkdbmxvb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gagqthczv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gipedsmkw.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/grcrjnrnk.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gipirspeb.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gltjonmob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gqtunyqmm.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gwmcuzdek.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gvyrfupia.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gyoepmuni.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gnzaslvgu.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gryhdayrx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gjoijqepj.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/ggauvckcv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gufyxukcr.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/ggeaeuxiu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gqxeeaiar.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gbtjhgwts.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gfqgxnpgx.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gcdycurvm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gfzzwjvjq.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gbjfjvmea.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gxjlzdlbw.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gzwwesime.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/ganborxod.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/goaqisxzy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gslszvrnr.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gfdsmsyre.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gwpitteiy.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gwhuqalaj.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gtguhjshk.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gtjyduios.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gqgiqawom.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdheasiu.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gvtejlcxd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/goybenkdl.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gfyhbzhrx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gxmtfehgn.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gdfecfktf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gwptgyuxe.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/ggzzaaajn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ghtvaiupc.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gqxhqwtjf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gtasgrgrp.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gdqrtsrxn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gvihgnput.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gunzxyims.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gmytnphla.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gjislzwzy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gdllicwpw.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gbmgimzlh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gmrdevuig.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/ghmeqxplv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/groxfxfhx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gaarjirli.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gcfndjgno.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/garamtzib.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/grvrutoez.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gheeafuwe.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gybhmnxwk.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/grlsyuadj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gsuetoqcw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/ggqagfrqr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gwftbwxkk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gxueppgoz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gxjxxjsln.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gkbbhxygi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gwlkhsluh.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/guxkrwgbf.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gybrrjhpi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gxmnuejar.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gbruipeew.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gotayfxvi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gdrraohqi.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gptxmjeuw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/grgonhkck.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gumcggmmv.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gctiohuqm.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gsrnwbjbu.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/guulkncwj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/guvqiqwbr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gckvbkfxa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gaeyltkid.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gcwsihrvq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gwqtevgxl.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gsgbxwpyu.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gjzxcahbw.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gvhzudnhg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gqorygxvy.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gbblmvjxf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gkefyvhnq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gumqcmjnk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/giqhgihma.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjgaznfkr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gzlybcmyh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdafaoxhm.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcpdbpytm.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gdsnpjobi.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gufhonjzg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gqxzrdosn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gbopkfbap.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gedccnsxo.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gsntenkke.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gdlaqcxjc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/givavxqyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/ggrpxddzv.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gnfscfsui.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gxafzdoaz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gtclgmmpk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gyhskhmob.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gqgoohgzm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxysuxegb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gxmlkmkem.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gzbpyxcrn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/glbhnjlbz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gfsbtovgj.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gmcspzuna.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/ggymeoxst.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/guhccpjeb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gcqvpskpo.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gwfmzmgqe.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gokamplho.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gkcbslgpy.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gfwzgayeu.sHtML


<!-- 参考信息 -->