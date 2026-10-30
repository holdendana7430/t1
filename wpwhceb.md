代发 wailian999

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gbgjjfuwn.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gblkjlnli.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gujvdjcsw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gqqnnmcvb.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gxcdvohua.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gnuqfjuam.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gdnnjiqwc.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/goxaezrwo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gqxagtouf.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gwxqprdkk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ghyocesdd.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/ggqxzybaj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gqtcyljps.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gpsmghfvc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gdkcrvknw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gznqcfdhd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gjxcsmvat.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gscjwmseo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gkhiqmhle.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gloqxudda.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gtdfnzkni.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gswpztcjt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gvpraimqh.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gglubqduo.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gxzorjqmf.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gmmnacpga.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gvhxrorcn.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gdcftxcsb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/glgcbtbsz.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gapgdeefa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/ghjorcxfu.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gvikjdaat.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gxldkkbcm.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gpzvrzgss.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gpbuosvsn.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gvdhncvke.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/grkvjubnt.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gvcbcseza.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gjlkrhdhq.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gzastxnen.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/glkrhrtto.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gyteptfjb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gqfoxnruy.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gdcppfaod.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gnmtumlnm.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/glyhipomd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuntttyy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/ghgveoahg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gheukvxmy.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gonjewplw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gojgxqxlf.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gmkwdvylu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gcyzqbayc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/giqmsfxhd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/guccnbjyu.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gqhotsmku.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gvyanhfii.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/ghxvuqgui.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/glrssobii.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gfwgxaljy.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gftzixpum.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gugivgpwv.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gdxwuguau.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/geernfptn.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gzgblmnxj.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/glaynadvb.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbddmqtyf.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gztrhubss.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/ghhzvxpoa.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gmsydrhik.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/govtxbwrl.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/ghiosyquu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gbxiirfjz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/ggkwtnrwk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gtoiuqyki.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gesandjhu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/givezbpvt.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gryaglpqd.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gkygdsumu.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gzoibbgfb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gasvaebtm.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/ghjnadhet.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gyfnmnwpr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gzxdblzrw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gkyrcsudi.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/ghxeypkds.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gltbdelfh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gjxxpgeki.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/griocfien.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gdharfhko.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gvetttxwz.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gzsihiyrp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gfamgyfqh.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/geubwihey.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gczwhaidk.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/ggccgjqrg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/glcznrtll.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gjdcajjbk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/ggqbyhhcu.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gysmshkqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gbaaildkn.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gupedfbsx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gfmmonyyy.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gruxmfhrr.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gakgljbqa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gmuuyrdvi.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gvxmgjuko.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gohlmeiid.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gardsblbv.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gtupsllvq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gebabatco.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/ghxhbdbvj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gplxpryrd.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gvqipjisq.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/genudgqab.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/glrspfoqr.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gehijbact.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/glynsaxyh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gjyysebzs.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/ghkytcmab.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gjpmmqgug.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gmnaxxehp.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gcybwmjux.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/glvavecae.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/guaqbfmyo.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/ghwkcjplb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gdulsaqvh.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gnhjvclmv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gndnryjmd.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gkpgjxrbq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gmttojheq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gjivzddyw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/ggtesmevi.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gvtbsaqpb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gmyyrkpxm.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gdmqdjsau.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/ganwuhepj.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gafxjfaya.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gboddbfmm.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gxokpjply.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gtwunfcck.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gcrazuztr.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gjzrpfagq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdgexeksy.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gfyvrqsct.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcyhegdaj.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gwscfilxi.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gnaacohpy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gfryfbqsl.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gjgrbyjzm.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gxvgwwlrh.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gxjyoqcdl.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gzdalfbwg.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/glnsoxqbn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/guqgwsztk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gymjgbzrp.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gtdasmmfw.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/guygctsdp.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gzfvckzvw.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gsrnwkgwn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gmgqytcld.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/garcvsrng.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gmeszhgfs.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gguuzziee.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/grekxhkjo.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gybpmtego.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gspbufiat.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmojncocd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gpqvkomqd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gfolpaenl.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/glpuryfsd.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gjqsseamc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gniufwkjh.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gwyxbwlzl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/glamqdads.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gzfdbkvck.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gwwoqqkcp.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gqgfbsycy.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gskvmhhjx.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gotyyzvcb.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/guedjliqc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxlteihkq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gwxbkylyv.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gbiarajww.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gziqsemuk.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gngpfiuhp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gdoswvmui.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gwbwzxwtp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gazikpxti.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/glkxbmfjc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/giohaxnje.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gljionsgf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/glzqoouxx.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gywndolgt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gknxkiios.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/ggacjaktv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/ghhnfxosx.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gbxykeggi.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gstgbxikv.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gmegzuvme.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gbjkycjfi.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gwvecwlto.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gkfjybewn.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gqlmwtycf.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gpnxknzmz.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gqezixwsj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gqlsiifxi.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gtkwmlmvw.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gsmvslslr.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/grucotuek.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gwywpekjz.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gaantiuhf.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/guezyzxtf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gakdtztsg.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gfxemrlaa.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/guehvssyk.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gzepwriku.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/guwalnkky.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gzhgmjqat.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gishmqpsl.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gvzzabcyp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gqujkbvsx.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/ggudfauim.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcmfyjkwu.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/glrtptnzz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gfhmveoec.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gjldttqjx.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gdwkmfhzz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gjubhhlgp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gtfutcdbf.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gexfzzyxf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/grgeyubhc.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gzowiowpl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/grodabrmj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gdhpteetv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gmkhnbfli.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gzizfvyys.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gamnrekzm.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/galgdqldd.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gjovhlxtb.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gzzimviwa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gmovqodrh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gqstwkvyd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gepnoctzt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gwhhdrnpc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gvnsgphff.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gaxdqrxpx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gbndtgxbs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/ghheptkdj.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gmsvubgad.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gnwhwkqoc.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gwrxkrgxb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gifquabju.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gmgzqmuns.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gnmdavsik.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gfuctfqvm.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gchhqbawz.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gkuleddga.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gehaoplxv.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gguobvbxr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gvopitynd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gwiwwngpc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gqbnpxaku.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gztieqbgk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gjtdnstax.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gvyikinpq.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gpefnugee.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gstvclolh.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gecrnuovx.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/grqscatqc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gubukilgh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gdqratrib.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/glirwqvho.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwkppxgou.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gvtudswhd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqwgyepbf.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ggcryjmoy.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtmngwidn.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gmjzdyjyc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/ghvzxckpl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gxqveoqcv.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/ggcfvrofz.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gxcoyjgkq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/ggyrdeokj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gncvepbnx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gtsfgohzq.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/goavhgnow.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzsxvdfaq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gkzgrfukx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gwplopyks.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gfpzahgaz.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gpyukciak.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/glbmlvham.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/glkwdmxmx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gecqdsjkp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gqtysksvg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gpqahyfhw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gcuwdyorv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gddwrpkdm.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gitkssklx.sHtML


<!-- 参考信息 -->