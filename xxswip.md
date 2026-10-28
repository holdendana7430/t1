代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xuanzx.com/gtvowpvmxo.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gtqhfheiiv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenzaomai.com/gtojdgtmqu.html

[R09] 字符串比较
来源：http://hz.9152youxi.cn/gtzgmitxbs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtlbqgxlxw.html

[R10] 正则匹配
来源：http://hz.feifeiyinyue.top/gthtbshkoq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shanyushiyangtech.top/gtgbrvzrxr.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtfypvnumy.html

case "$1" in
来源：http://hz.nanxuanxn.top/gtuxcxyalj.html

start) echo "启动" ;;
来源：http://hz.zhijiandao.cn/gtshyqoawz.html

stop)  echo "停止" ;;
来源：http://hz.yuxming.cn/gtxvhmlaxg.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258888.top/gtxnwtzajn.html

esac
来源：http://hz.yanxiufei.cn/gtfcyqrpig.html

[R12] for 遍历文件
来源：http://hz.hnqzz.top/gtbgmcvcrf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.kuanghao11.cn/gtikfdxjyh.html

[R13] for 计数循环
来源：http://hz.jianghu66.top/gtnzpcaoxz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtwzxnxqet.html

[R14] C 风格 for
来源：http://hz.fengsongda.top/gttvvhzkcq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtizozlhdx.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gttedazpki.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ywan-chungtsiang.top/gtaejjhzlw.html

[R16] until 等待条件
来源：http://hz.jinyuanbaomall.cn/gtwkszdhsq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daria6918.cn/gtcrwaedwy.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtettvainr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hammf.cn/gtoruutosq.html

[R18] 遍历数组
来源：http://hz.nanxuanxn.top/gtesuqhomw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtqclzepvl.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtzqzwftaw.html

echo "${#arr[@]}"
来源：http://hz.shzxlz.cn/gtxszmxbzi.html

[R20] 关联数组（字典）
来源：http://hz.dashuyun.cn/gtaelkpqbl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtxbgtqkci.html

[R21] 字符串长度
来源：http://hz.316326.xyz/gtixaisghg.html

echo "${#s}"
来源：http://hz.xuanzx.com/gtnddgmles.html

[R22] 截取子串
来源：http://hz.sweek.top/gtxagyayxa.html

echo "${s:0:5}"
来源：http://hz.jinghuilouyu.cn/gtllpxjuwv.html

[R23] 字符串替换
来源：http://hz.yanxiufei.cn/gtacjmywad.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtkjapfzhr.html

[R24] 大小写转换
来源：http://hz.hammf.cn/gtpcbxpfin.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tanke756.top/gtudthccyv.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigfzy.top/gtnxnsuuga.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtoywtqjee.html

[R26] 命令替换
来源：http://hz.tanke756.top/gtehfkldne.html

now=$(date +%F); echo "$now"
来源：http://hz.jinyuanbaomall.cn/gtzknduswc.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gtzfnsrvvo.html

echo $((1 + 2 * 3))
来源：http://hz.gaohongyu789.top/gtbwevrunu.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtejfinioc.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenlongwang.top/gtcaxjpwhc.html

[R29] 定义函数
来源：http://hz.cashguo.top/gtcvfqfqfu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtpgmioqor.html

[R30] 函数返回状态码
来源：http://hz.birdmap.top/gthuvolxjy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fzhhl.top/gtqbrmlwig.html

[R31] 局部变量
来源：http://hz.ywan-chungtsiang.top/gtlfywdwje.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgufenzy.top/gtdfrkoyrc.html

[R32] 参数个数校验
来源：http://hz.hammf.cn/gtulzutqhm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hfpthk.cn/gtftvjvjre.html

[R33] 捕获错误并提示行号
来源：http://hz.vqdsnc.cn/gtafvxemho.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhijiandao.cn/gtknwntxmk.html

[R34] 退出时清理
来源：http://hz.jqgfzy.top/gtpgrwxeoe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtbhksfjix.html

[R35] 后台执行并等待
来源：http://hz.sysykeji.top/gtqurwshyf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhongyouzk.top/gtcdajjsfz.html

[R36] 并发执行多个任务
来源：http://hz.bjfxy.top/gteplhgjbg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnxiangtu.top/gtdgksnyov.html

[R37] 把输出赋给变量
来源：http://hz.gogol.net.cn/gtdlzlwgfl.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gthzmzmlyf.html

[R38] 管道串联
来源：http://hz.yueranfly.top/gtjydzypyz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.9152youxi.cn/gtogpdtcsz.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gtszrfbkws.html

cmd > out.log 2>&1
来源：http://hz.jqgfzy.top/gtmezlkxdr.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gtxsgtfvxl.html

echo "log" >> out.log
来源：http://hz.bjfxy.top/gtgahoadgb.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtwmdgkwjn.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtsykhujmy.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gtheusxyrk.html

wc -l < a.txt
来源：http://hz.pengpengdd.cyou/gtoyhmoken.html

[R43] 按名字查找文件
来源：http://hz.yongpay.top/gtbsmrttlm.html

find . -name "*.log" -type f
来源：http://hz.guannengcc.top/gtkumfxgmm.html

[R44] 按修改时间查找
来源：http://hz.yuanzhike.top/gtuuyeewno.html

find . -mtime -7 -type f
来源：http://hz.fzhhl.top/gtpxjmvgec.html

[R45] 批量删除
来源：http://hz.yuanzhike.top/gtqqxmuvru.html

find . -name "*.tmp" -delete
来源：http://hz.zhijiandao.cn/gtwycyzigd.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangtech.top/gtmurfxmvm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gaohongyu789.top/gtzunnuimm.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gtdfzpblde.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtnhlsdnjl.html

[R48] awk 取指定列
来源：http://hz.tian-w.cn/gtvpcrfzex.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtlzucwxcr.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtshfqqbca.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtrfpolbmi.html

[R50] awk 求和
来源：http://hz.tanke756.top/gtjpamorkx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhixingplan.top/gtsmatbwlr.html

[R51] 排序去重取前几
来源：http://hz.guowangkeji.top/gtbclncaug.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtmuuwlzfs.html

[R52] 统计行数
来源：http://hz.jiagoushi.top/gtbjmqunzg.html

wc -l a.txt
来源：http://hz.pycfn.com/gtyjvakicb.html

[R53] 查看文件头与实时尾
来源：http://hz.xingfuxueyuan.xyz/gtglmmuuwo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtudqkwtne.html

[R54] 比较两个文件
来源：http://hz.hammf.cn/gtizjpbtzy.html

diff a.txt b.txt
来源：http://hz.jinqigfzy.top/gtdsyxnvvl.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtscgbuqpb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.meibo888.top/gtpuiemmgd.html

[R56] 远程拷贝
来源：http://hz.jiagoushi.top/gtpsumkiql.html

scp file user@host:/path/
来源：http://hz.zycfv.cn/gtlyglcuom.html

[R57] 远程执行命令
来源：http://hz.guannengcc.top/gttacptdkf.html

ssh user@host 'uptime'
来源：http://hz.zhengqikj.top/gtrzghdrle.html

[R58] 下载文件
来源：http://hz.zhoulong.xyz/gtjwggquio.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtzmyeezgw.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtewjnyfcq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.kuanghao11.cn/gthaybtzyg.html

[R60] 只看 HTTP 状态码
来源：http://hz.snrcjt.cn/gtoyxxcdyw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yongpay.top/gttzrraehp.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gthzfbtpfu.html

df -h;  du -sh *
来源：http://hz.zycfv.cn/gtrxmfplek.html

[R62] 找最占空间的文件
来源：http://hz.vqdsnc.cn/gtfjxtxwht.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtibybwgll.html

[R63] 内存与进程
来源：http://hz.daxiang520.top/gtdpxoxmzd.html

free -h;  ps aux | grep nginx
来源：http://hz.birdmap.top/gtyjdumxim.html

[R64] 结束进程
来源：http://hz.zhijiandao.cn/gtmprjgptj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtbenwtrop.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gtrbzysetl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtnkgkcqxt.html

[R66] 定时任务
来源：http://hz.aizwys.cn/gtvyrnovjf.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangtech.top/gtwyxelmdk.html

[R67] 生成随机十六进制串
来源：http://hz.sxryk.cn/gtcfoyrzwh.html

openssl rand -hex 16
来源：http://hz.wangdashe.top/gtppxyzxgs.html

[R68] 计算文件校验值
来源：http://hz.xziqi.cn/gtftsxjbou.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xziqi.cn/gtyzzkdwqj.html

[R69] 生成随机密码
来源：http://hz.gogol.net.cn/gtmxwpgroo.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258888.top/gtnkocxsun.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtngtkqlyy.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtqiqtwzsd.html

[R71] 日期格式化
来源：http://hz.cqqwz.cn/gtvnhifezw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guannengcc.top/gtmovrwfbm.html

[R72] 等待端口就绪
来源：http://hz.yj20258888.top/gtkqvevztc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenlongwang.top/gtwkewmmop.html

[R73] 分割大日志
来源：http://hz.jlsjyb.cn/gtkpeqjwmw.html

split -l 1000 big.log part_
来源：http://hz.snrcjt.cn/gtxczwlpdu.html

[R74] 批量重命名
来源：http://hz.jinqigufen.top/gtusswhasd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgfzy.top/gtdmaulwvz.html

[R75] 导出环境变量
来源：http://hz.xuanzx.com/gtnzgaxnei.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gtadkvukmj.html

[R76] 使用临时文件
来源：http://hz.pengpengdd.cyou/gtonrjsarh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtembpzokc.html

[R77] 读取用户输入
来源：http://hz.jinyuanbaomall.cn/gtwjngaumy.html

read -rp "请输入: " ans
来源：http://hz.gzhubu.top/gtzudzzjop.html

[R78] 交互式菜单
来源：http://hz.guannengcc.top/gtteautlav.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pengpengdd.cyou/gtuyyibrgw.html

[R79] 解析命令行选项
来源：http://hz.chenjidiqi.icu/gtgzgjyvtr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dianchejie.cn/gtiyyijzlx.html

[R80] 查看脚本执行耗时
来源：http://hz.svipenyu.cn/gtgoypwblu.html

time ./run.sh
来源：http://hz.vqdsnc.cn/gtrjhofxdo.html

================================================================================
来源：http://hz.birdmap.top/gtkypcodpu.html

S. C / C++ 专题
来源：http://hz.tianlin.xyz/gtzpcudjwi.html

================================================================================
来源：http://hz.dianchejie.cn/gtymshuogc.html

[S01] C：Hello World
来源：http://hz.xylfe.cn/gtfwynxktd.html

#include <stdio.h>
来源：http://hz.jiagoushi.top/gtuefnhhbo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sxryk.cn/gtljvkfypr.html

[S02] C：变量与格式化输出
来源：http://hz.meibo888.top/gtfizwdphm.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangkeji.top/gthqlppows.html

[S03] C：读入整数
来源：http://hz.smart0.xyz/gtyuwzzuea.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gthfggbsqd.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtwlphrnva.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gaohongyu789.top/gtbxswnihq.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gttcbfqurl.html

strlen(s)
来源：http://hz.xuanzx.com/gtidrjwcyf.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtcduupbim.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangtech.top/gttczlynua.html

[S07] C：数组遍历求和
来源：http://hz.ydjk.org.cn/gtwlxsbdwm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gtnteuhwqi.html

[S08] C：动态内存分配与释放
来源：http://hz.yuxming.cn/gtsfhznupy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuxming.cn/gtprgsngqt.html

[S09] C：结构体定义与初始化
来源：http://hz.aizwys.cn/gtgnspvqpv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258888.top/gtwslaulgg.html

[S10] C：指针与解引用
来源：http://hz.snrcjt.cn/gtunedetlk.html

int *p = &a;  *p = 5;
来源：http://hz.yuxming.cn/gtbwzujdth.html

[S11] C：逐行读文件
来源：http://hz.xuanzx.com/gtxhkvpevz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.andypj.xyz/gtttcxzglr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhixingplan.top/gtpfemozxs.html

fclose(f);
来源：http://hz.hnqzz.top/gtuptfordg.html

[S12] C：写文件
来源：http://hz.guowangkeji.top/gtxklkkcmd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangdashe.top/gtnwvbzfhm.html

[S13] C：宏定义
来源：http://hz.chenjidiqi.icu/gtrqreuhfo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.52xcode.cn/gtoaidbyfb.html

[S14] C：枚举
来源：http://hz.nanxuanxn.top/gtkyhlfzir.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258.top/gtbqdwvwds.html

[S15] C：类型转换
来源：http://hz.zycfv.cn/gtkusueujk.html

(double) a / b
来源：http://hz.tianlin.xyz/gtamshmwvs.html

[S16] C：位操作置位
来源：http://hz.hfpthk.cn/gtshibsvhl.html

x |= (1 << 3);
来源：http://hz.zhaomingkeji.xyz/gtsmtwbcre.html

[S17] C：安全拼接字符串
来源：http://hz.svipenyu.cn/gttbquqdeq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.316326.xyz/gtlpawhiwa.html

[S18] C：命令行参数
来源：http://hz.yvedp.cn/gtmyvihiqb.html

int main(int argc, char **argv)
来源：http://hz.fzhhl.top/gtdbqeezah.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gtigsfkamd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtjhigyezx.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtbqzoahbs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtzfetuewd.html

[S21] C：字符类别判断
来源：http://hz.zhijiandao.cn/gtawkgxfsw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hysaishi.cn/gtagxakjvz.html

[S22] C：字符串转数字
来源：http://hz.ybcxt.top/gtolznvxwe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guannengcc.top/gtriiavirf.html

[S23] C：随机数
来源：http://hz.wangdashe.top/gtnpjdzhxi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shuidangran.top/gtkivyldvc.html

[S24] C：获取本地时间
来源：http://hz.zhijiandao.cn/gttybhiwzf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jiagoushi.top/gttsdafwev.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtdwagfzgb.html

memcpy(dst, src, n);
来源：http://hz.yj20258888.top/gtbudyjxlz.html

[S26] C：内存清零
来源：http://hz.hnqzz.top/gtizwqjqrm.html

memset(a, 0, sizeof a);
来源：http://hz.yuxming.cn/gtnpzmypsu.html

[S27] C：定义常量
来源：http://hz.yanxiufei.cn/gtuuqeffsu.html

const double PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtvgbdljdw.html

[S28] C：静态变量
来源：http://hz.yangfankeji.com/gtiqgfphyp.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtqttnfcbf.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtndratlud.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtgbuwbktg.html

[S30] C：头文件保护
来源：http://hz.andypj.xyz/gtrgaslror.html

#ifndef X_H
来源：http://hz.yj20258.top/gtxcrenckc.html

#define X_H
来源：http://hz.daria6918.cn/gtapizodud.html

#endif
来源：http://hz.guannengcc.top/gtgavnbctf.html

[S31] C++：Hello World
来源：http://hz.kuanghao11.cn/gtseffbocj.html

#include <iostream>
来源：http://hz.quarkkingdee.top/gtzxqgxont.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnqzz.top/gtnwfmciuo.html

[S32] C++：字符串
来源：http://hz.hfpthk.cn/gtqdmltkpf.html

std::string s = "hi";  s += "!";
来源：http://hz.cheryme.top/gtunhchqss.html

[S33] C++：vector 增删
来源：http://hz.jianghu66.top/gtzuisnwma.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gtccgwnrfv.html

[S34] C++：遍历 vector
来源：http://hz.zhixingplan.top/gtcmvyysif.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.snrcjt.cn/gtnnzdeeet.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gtbivkkbyh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtulvollym.html

[S36] C++：unordered_map
来源：http://hz.jlsjyb.cn/gtxuxdmgkz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtlfnnwpsg.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtyhiueshb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.meibo888.top/gtsdtvqczu.html

[S38] C++：排序
来源：http://hz.jqgfzy.top/gtqdorrqjo.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtxiewuukb.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtzyjzsqqs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuxming.cn/gtzchhdnxn.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gthwrmmzvi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.svipenyu.cn/gthjvwdzoi.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtarwqtqbp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258.top/gtbseqvbkb.html

[S42] C++：继承与虚函数
来源：http://hz.zhiwuduotai.top/gtxpkdtrkg.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydzc1.top/gtetlqnwlm.html

[S43] C++：智能指针
来源：http://hz.dianchejie.cn/gtbvqicggg.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtgkmdeqjv.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gtvzlfvavj.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtvhgvwqsy.html

[S45] C++：lambda
来源：http://hz.ybcxt.top/gtvntvpayd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hywenlv.cn/gtyzvgkrxy.html

[S46] C++：函数模板
来源：http://hz.pycfn.com/gtonpavokq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ppjwa.cn/gtgsurbtki.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhixingplan.top/gtlipigaoy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtwduuzakl.html

[S48] C++：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtyxdaemkd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtkoyyydto.html

while (std::getline(in, line)) { }
来源：http://hz.pengpengdd.cyou/gtmadqugii.html

[S49] C++：写文件
来源：http://hz.hnxiangtu.top/gtjoyierqm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guannengcc.top/gtgmtzmtkh.html

[S50] C++：格式化数字
来源：http://hz.nanxinkj.top/gtfrpshqds.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangdashe.top/gtkscjxrzb.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtrkhsukxc.html

static_cast<double>(a) / b
来源：http://hz.0kj1m.cn/gtedxmlbdj.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtzxdtkbsm.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtsohannsm.html

[S53] C++：移动语义
来源：http://hz.chenjidiqi.icu/gtqqjpzlca.html

std::vector<int> w = std::move(v);
来源：http://hz.cdnleiting.top/gtmmhjwwqy.html

[S54] C++：异常处理
来源：http://hz.sysykeji.top/gtmppnbqiv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhaomingkeji.xyz/gtfftwycsl.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtsbksrsyo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.birdmap.top/gtrxvjnkaq.html

[S56] C++：optional
来源：http://hz.shanyushiyangtech.top/gtabdfclhg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sxryk.cn/gttuvwrhxf.html

[S57] C++：编译期常量
来源：http://hz.zhiwuduotai.top/gtohfsfksj.html

constexpr int N = 10;
来源：http://hz.quarkkingdee.top/gtnqxmbiei.html

[S58] C++：命名空间
来源：http://hz.xinyue.icu/gtfnfojhkr.html

namespace ns { int f() { return 1; } }
来源：http://hz.smart0.xyz/gtwrekluen.html

[S59] C++：静态断言
来源：http://hz.redwolf501.top/gtyxjpnajw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hysaishi.cn/gthpxjcpvp.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtdwqaadze.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtmrxzahnw.html

================================================================================
来源：http://hz.nwbrower.top/gtilkqtimy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtkhcsnhnp.html

================================================================================
来源：http://hz.52xcode.cn/gtfedvyorb.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtqknqqchx.html

println("Hello")
来源：http://hz.52xcode.cn/gtzkabuhwy.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtpxlzzugn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gaohongyu789.top/gtbiesqjgi.html

[T03] Kotlin：字符串模板
来源：http://hz.guannengcc.top/gtlutewsrl.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtkujpurlm.html

[T04] Kotlin：空安全
来源：http://hz.kuanghao11.cn/gtxxfalsfe.html

val n: String? = null;  n?.length
来源：http://hz.yj20258.top/gtizvklhxt.html

[T05] Kotlin：when 表达式
来源：http://hz.ivvv.top/gthrteztvu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tianlin.xyz/gtesgavrcz.html

[T06] Kotlin：集合映射
来源：http://hz.wangdashe.top/gtmmdslfpc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.havefunace.top/gtrlvovkia.html

[T07] Kotlin：集合过滤
来源：http://hz.cashguo.top/gtrnuneway.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gteyqsgwuh.html

[T08] Kotlin：数据类
来源：http://hz.sufxvd.cn/gtoxwrenps.html

data class User(val name: String, val age: Int)
来源：http://hz.zhixingplan.top/gtnhpyunir.html


<!-- 参考信息 -->