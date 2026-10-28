代发 wailian999

readonly PI=3.14
来源：http://hz.redwolf501.top/gtnqrwlkvf.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtqxeuqjob.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhaomingkeji.xyz/gtzknrbfxc.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gtedhnrzge.html

name="${1:-default}"
来源：http://hz.shangyingyoupin.top/gtqkbylanr.html

[R06] 判断命令是否存在
来源：http://hz.zycfv.cn/gtihiimnxw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daxiang520.top/gtatjbaftg.html

[R07] if 判断文件
来源：http://hz.9152youxi.cn/gtuatsauvh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.vqdsnc.cn/gtgbyclzfs.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtqlhuczog.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.vqdsnc.cn/gtzutmmgiz.html

[R09] 字符串比较
来源：http://hz.andypj.xyz/gtwkoxnjlb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dianchejie.cn/gtvptmqnxv.html

[R10] 正则匹配
来源：http://hz.kuanghao11.cn/gtwrnwkmuu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuanzhike.top/gtnvchpwss.html

[R11] case 多分支
来源：http://hz.jyoumei.cn/gtxeoyqgdp.html

case "$1" in
来源：http://hz.havefunace.top/gtzmzcjgio.html

start) echo "启动" ;;
来源：http://hz.ybcxt.top/gtdylqqcyc.html

stop)  echo "停止" ;;
来源：http://hz.jqgufenzy.top/gtrhuldlgu.html

*)     echo "未知命令" ;;
来源：http://hz.andypj.xyz/gtysodnfii.html

esac
来源：http://hz.iojbl.cn/gtqwjtmwlu.html

[R12] for 遍历文件
来源：http://hz.jqgufenzy.top/gtruecbvaw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sufxvd.cn/gtydfccpzg.html

[R13] for 计数循环
来源：http://hz.guowangkeji.top/gtrpkcwhes.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtfaxoalhx.html

[R14] C 风格 for
来源：http://hz.xuanzx.com/gtgnipqnss.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gtrcjlktms.html

[R15] while 逐行读文件
来源：http://hz.wangshuangyany.cn/gtniqmoyha.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hysaishi.cn/gtmqdeemmf.html

[R16] until 等待条件
来源：http://hz.tian-w.cn/gtjfpjhsoq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aizwys.cn/gtnumqqsme.html

[R17] 数组定义与取值
来源：http://hz.ywan-chungtsiang.top/gtvkmzaqjp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gtsyganpio.html

[R18] 遍历数组
来源：http://hz.xinyue.icu/gtqambcwzo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtrrvjiyrs.html

[R19] 数组长度
来源：http://hz.jyoumei.cn/gtgditclaz.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtieufitpb.html

[R20] 关联数组（字典）
来源：http://hz.ehwqpu.com/gtgyllhoxr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gtaspknrou.html

[R21] 字符串长度
来源：http://hz.jiagoushi.top/gtuydjkgde.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtupqweyip.html

[R22] 截取子串
来源：http://hz.yvedp.cn/gtftyuwguy.html

echo "${s:0:5}"
来源：http://hz.ivvv.top/gtloezcltp.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtjvzwtxuz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gtnqfvmbav.html

[R24] 大小写转换
来源：http://hz.yj20258888.top/gtmkevunbp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtjdnuigid.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtguwkipna.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guowangkeji.top/gtaxfsayca.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtsbalktdu.html

now=$(date +%F); echo "$now"
来源：http://hz.hnxiangtu.top/gtaztxgfzc.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gtfenpbrpf.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtexlefqah.html

[R28] 浮点运算
来源：http://hz.bjfxy.top/gtbczlgfon.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhijiandao.cn/gtiabceikt.html

[R29] 定义函数
来源：http://hz.havefunace.top/gtwdkjpzqo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxinkj.top/gtprfdmfhu.html

[R30] 函数返回状态码
来源：http://hz.gzhubu.top/gtuxknweue.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258.top/gtvyyffyql.html

[R31] 局部变量
来源：http://hz.jqgufenzy.top/gtnkoyyrsp.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gtofkppgnn.html

[R32] 参数个数校验
来源：http://hz.jqgfzy.top/gtdazrsytw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtyumksbkl.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtoktmiiwg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yueranfly.top/gtucejzahu.html

[R34] 退出时清理
来源：http://hz.sxryk.cn/gttbxbfusy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gttfslecwf.html

[R35] 后台执行并等待
来源：http://hz.fengsongda.top/gtecxfhwwy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangshuangyany.cn/gtkwecfynm.html

[R36] 并发执行多个任务
来源：http://hz.jinqigfzy.top/gtvnjlmbff.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yanxiufei.cn/gtixyisogx.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtfrpocsyd.html

files=$(ls -1)
来源：http://hz.guowangkeji.top/gtiuepbwmb.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gtyyxihqqz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pengpengdd.cyou/gttyvsdvvu.html

[R39] 重定向标准输出与错误
来源：http://hz.xuetiantiany.cn/gtfdgdqvde.html

cmd > out.log 2>&1
来源：http://hz.ppjwa.cn/gtqnlfogtj.html

[R40] 追加写日志
来源：http://hz.tanke756.top/gttpjytzwu.html

echo "log" >> out.log
来源：http://hz.jiagoushi.top/gtpoqpmkua.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtmgnhazxg.html

cmd >/dev/null 2>&1
来源：http://hz.xuanzx.com/gtjtumhlrd.html

[R42] 输入重定向
来源：http://hz.ppjwa.cn/gtmwdbnunx.html

wc -l < a.txt
来源：http://hz.shuidangran.top/gtyaezitao.html

[R43] 按名字查找文件
来源：http://hz.nanxinkj.top/gtlfdoxugw.html

find . -name "*.log" -type f
来源：http://hz.yonumen.top/gtiufckvfo.html

[R44] 按修改时间查找
来源：http://hz.hnxiangtu.top/gtnjgqkxsm.html

find . -mtime -7 -type f
来源：http://hz.shuidangran.top/gtvynrhsbz.html

[R45] 批量删除
来源：http://hz.tianlin.xyz/gttgswarao.html

find . -name "*.tmp" -delete
来源：http://hz.haohaochexian.top/gtrywmpuap.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gttefddctp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fzhhl.top/gtkzgdxmey.html

[R47] sed 单行替换
来源：http://hz.fengsongda.top/gtdyrlaeim.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gtwbrjejwj.html

[R48] awk 取指定列
来源：http://hz.xziqi.cn/gtxyukrban.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnxiangtu.top/gtklhpumau.html

[R49] awk 带条件
来源：http://hz.nanxuanxn.top/gtmseihaoz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenlongwang.top/gtaqhppauc.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtkmmohcxj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenlongwang.top/gtedsjpnoc.html

[R51] 排序去重取前几
来源：http://hz.zhiwuduotai.top/gtcwlbiwol.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.haohaochexian.top/gtdsotazmy.html

[R52] 统计行数
来源：http://hz.shzxlz.cn/gtfuxczrrm.html

wc -l a.txt
来源：http://hz.sweek.top/gthehqaihc.html

[R53] 查看文件头与实时尾
来源：http://hz.fengsongda.top/gtprwsrvsy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtnrcsyist.html

[R54] 比较两个文件
来源：http://hz.feifeiyinyue.top/gtnyfmvsfq.html

diff a.txt b.txt
来源：http://hz.316326.xyz/gtmknvvvkh.html

[R55] 压缩与解压
来源：http://hz.zhijiandao.cn/gtxdxyosbe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.0kj1m.cn/gtnnitntzk.html

[R56] 远程拷贝
来源：http://hz.hnxiangtu.top/gtevluztco.html

scp file user@host:/path/
来源：http://hz.chenjidiqi.icu/gtxbdikffw.html

[R57] 远程执行命令
来源：http://hz.yj20258.top/gtvdawcamn.html

ssh user@host 'uptime'
来源：http://hz.meibo888.top/gtlxastnkn.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtthydlsqh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigufen.top/gtycfaicev.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gthupqeadi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtvczbhfoi.html

[R60] 只看 HTTP 状态码
来源：http://hz.tian-w.cn/gtjbbjjkoo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dashuyun.cn/gthwtbnamw.html

[R61] 磁盘占用
来源：http://hz.yanxiufei.cn/gtdicmkwtb.html

df -h;  du -sh *
来源：http://hz.cheryme.top/gtqflopqpu.html

[R62] 找最占空间的文件
来源：http://hz.ivvv.top/gtirfwleuy.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtiawjjqfd.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtunhvwyjy.html

free -h;  ps aux | grep nginx
来源：http://hz.cqqwz.cn/gtlcckxfsx.html

[R64] 结束进程
来源：http://hz.iojbl.cn/gtujllrflt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jiagoushi.top/gtyubxbpbd.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtzbugolii.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yvedp.cn/gtfitzmlrd.html

[R66] 定时任务
来源：http://hz.dianchejie.cn/gtqhrdwkqy.html

crontab -e;  crontab -l
来源：http://hz.kuanghao11.cn/gtkksklcox.html

[R67] 生成随机十六进制串
来源：http://hz.yangfankeji.com/gtydamrxiy.html

openssl rand -hex 16
来源：http://hz.yuanzhike.top/gttfvrwwky.html

[R68] 计算文件校验值
来源：http://hz.yj202588.top/gtdspsqujr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtpgnshhcn.html

[R69] 生成随机密码
来源：http://hz.cucudq.cn/gtpuwomuwm.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtvdhdbiyi.html

[R70] 时间戳与互转
来源：http://hz.jinghuilouyu.cn/gtzjobyppr.html

date +%s;  date -d @1700000000
来源：http://hz.shangyingyoupin.top/gtmltddufo.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtahkibiyg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.9152youxi.cn/gtvfgsczzd.html

[R72] 等待端口就绪
来源：http://hz.yongpay.top/gtxrpkdqqr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtrtcebqcu.html

[R73] 分割大日志
来源：http://hz.pengpengdd.cyou/gtuwfvsjfz.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtvdrqzuei.html

[R74] 批量重命名
来源：http://hz.0kj1m.cn/gtuamnbpwv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pycfn.com/gtwctshviv.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtkllwtfsp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtumysjroa.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtmkchnegj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtohrohmin.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtmnxnrhdn.html

read -rp "请输入: " ans
来源：http://hz.yj20258.top/gtxaxixiiu.html

[R78] 交互式菜单
来源：http://hz.dashuyun.cn/gtdofatelm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guowangkeji.top/gtwlghdlhi.html

[R79] 解析命令行选项
来源：http://hz.jinqigfzy.top/gtubzubpkq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shuidangran.top/gtqfgssbpq.html

[R80] 查看脚本执行耗时
来源：http://hz.zhaomingkeji.xyz/gtuqblbgco.html

time ./run.sh
来源：http://hz.hnxiangtu.top/gtnsaseqvu.html

================================================================================
来源：http://hz.yangfankeji.com/gtuqrrxfws.html

S. C / C++ 专题
来源：http://hz.haohaochexian.top/gtryqiibvh.html

================================================================================
来源：http://hz.bjfxy.top/gtaugluzkc.html

[S01] C：Hello World
来源：http://hz.snrcjt.cn/gtqhdadhrf.html

#include <stdio.h>
来源：http://hz.sysykeji.top/gtzadgtpmh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuanzhike.top/gtmyxcmjjj.html

[S02] C：变量与格式化输出
来源：http://hz.sufxvd.cn/gtbnadnwtc.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gtfwifkhlx.html

[S03] C：读入整数
来源：http://hz.tanke756.top/gtlzqlyjwx.html

int x; scanf("%d", &x);
来源：http://hz.gaohongyu789.top/gtvhszdebg.html

[S04] C：字符串复制
来源：http://hz.nanxuanxn.top/gtwrdjnyjg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gzhubu.top/gtgxismhlj.html

[S05] C：字符串长度
来源：http://hz.nanxuanxn.top/gtmogszftr.html

strlen(s)
来源：http://hz.316326.xyz/gtykcpdflt.html

[S06] C：字符串比较
来源：http://hz.aizwys.cn/gtfpdamybm.html

strcmp(a, b) == 0
来源：http://hz.nanxuanxn.top/gtsqcvwdyn.html

[S07] C：数组遍历求和
来源：http://hz.cqqwz.cn/gtjaznlsvd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigfzy.top/gtrjxpoutn.html

[S08] C：动态内存分配与释放
来源：http://hz.sufxvd.cn/gthzzoqxhn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtuwiillvj.html

[S09] C：结构体定义与初始化
来源：http://hz.yuanzhike.top/gtvxjzkxgz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tianlin.xyz/gttdnbvhdc.html

[S10] C：指针与解引用
来源：http://hz.yj20258.top/gtcrhszwji.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtevhrmnpw.html

[S11] C：逐行读文件
来源：http://hz.xinyue.icu/gtsvueaigu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.iojbl.cn/gtwbynbiwt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sweek.top/gtussvznjb.html

fclose(f);
来源：http://hz.svipenyu.cn/gtupqgebkb.html

[S12] C：写文件
来源：http://hz.shzxlz.cn/gtyfjgjofd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nwbrower.top/gtuofdsdlb.html

[S13] C：宏定义
来源：http://hz.tian-w.cn/gtuazozafi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtcqgzggeh.html

[S14] C：枚举
来源：http://hz.wangdashe.top/gthvofygwh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtxoafwymq.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtaaeibcut.html

(double) a / b
来源：http://hz.nwbrower.top/gtgtgayrcc.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gtpdyjuuye.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gtloossaua.html

[S17] C：安全拼接字符串
来源：http://hz.jinghuilouyu.cn/gtlceygvcg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258.top/gtcxdgklxe.html

[S18] C：命令行参数
来源：http://hz.c1oappe.top/gteuthrrqe.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtbotzezup.html

[S19] C：快速排序
来源：http://hz.sxryk.cn/gtxrojkiai.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtuupaqhze.html

[S20] C：二分查找
来源：http://hz.tanke756.top/gtjqfhsstp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtywtwvlvc.html

[S21] C：字符类别判断
来源：http://hz.xinyue.icu/gtawqpyabd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hysaishi.cn/gtbgyaoqgr.html

[S22] C：字符串转数字
来源：http://hz.fengsongda.top/gtxhhssitv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhengqikj.top/gtepouqnna.html

[S23] C：随机数
来源：http://hz.9152youxi.cn/gtamqivjpl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgfzy.top/gtrlnwrhot.html

[S24] C：获取本地时间
来源：http://hz.quarkkingdee.top/gtgnzjfwob.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhixingplan.top/gtyefeacmb.html

[S25] C：内存拷贝
来源：http://hz.aibaodan.cn/gtwimujydy.html

memcpy(dst, src, n);
来源：http://hz.hfpthk.cn/gtmhtztcdi.html

[S26] C：内存清零
来源：http://hz.ydjk.org.cn/gtqivymupi.html

memset(a, 0, sizeof a);
来源：http://hz.zhijiandao.cn/gtufqtstyo.html

[S27] C：定义常量
来源：http://hz.nanxinkj.top/gtjrclmmza.html

const double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtvidqxmli.html

[S28] C：静态变量
来源：http://hz.mhx1999.top/gtdcspmxwy.html

static int counter = 0;
来源：http://hz.ivvv.top/gtxoayicpi.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtxwpjzqvz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgufenzy.top/gtjtksfqsl.html

[S30] C：头文件保护
来源：http://hz.yonumen.top/gtdjjcvbtc.html

#ifndef X_H
来源：http://hz.hywenlv.cn/gtgebppqom.html

#define X_H
来源：http://hz.fzhhl.top/gtluqpizzd.html

#endif
来源：http://hz.cucudq.cn/gtcfuwyskj.html

[S31] C++：Hello World
来源：http://hz.gogol.net.cn/gtzzyakygk.html

#include <iostream>
来源：http://hz.guowangkeji.top/gtyhhbznba.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.9152youxi.cn/gtahvilybk.html

[S32] C++：字符串
来源：http://hz.fengsongda.top/gtcnwlbmzd.html

std::string s = "hi";  s += "!";
来源：http://hz.zhixingplan.top/gtffutmyet.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtmngxcipb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fengsongda.top/gtoyljyrpz.html

[S34] C++：遍历 vector
来源：http://hz.yuanzhike.top/gttzidouya.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj202588.top/gtijbnqcqd.html

[S35] C++：map
来源：http://hz.sweek.top/gtpcipthli.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtonyaarkl.html

[S36] C++：unordered_map
来源：http://hz.daxiang520.top/gtnzjinnhu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtdgmrnjpn.html

[S37] C++：set
来源：http://hz.hnxiangtu.top/gtlfrrslet.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yangfankeji.com/gtssoyukto.html

[S38] C++：排序
来源：http://hz.zhixingplan.top/gtaaxvfwow.html

std::sort(v.begin(), v.end());
来源：http://hz.yj202588.top/gtkomecezu.html

[S39] C++：自定义比较器排序
来源：http://hz.zhixingplan.top/gtsypbnzsa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.kuanghao11.cn/gtuoskwmen.html

[S40] C++：查找元素
来源：http://hz.cucudq.cn/gtilwvmcfq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigufen.top/gtjvmzgaoy.html

[S41] C++：类与构造函数
来源：http://hz.9152youxi.cn/gtibgyogxc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aibaodan.cn/gtpbuqcsbu.html

[S42] C++：继承与虚函数
来源：http://hz.gotoacloud.top/gtsxiflyyd.html

class B : public Base { public: void f() override {} };
来源：http://hz.aizwys.cn/gtxuqqfnlf.html

[S43] C++：智能指针
来源：http://hz.nanxuanxn.top/gtchsfygjp.html

auto p = std::make_unique<int>(5);
来源：http://hz.yongpay.top/gtuzqsjwvv.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtyeitqbjd.html

void inc(int &x) { ++x; }
来源：http://hz.xuanzx.com/gtxxbekydo.html

[S45] C++：lambda
来源：http://hz.shangyingyoupin.top/gtlolmzhdj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtphbjmqyw.html

[S46] C++：函数模板
来源：http://hz.nanxinkj.top/gtvgfvcyph.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guowangkeji.top/gtnpuqgwzl.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinyuanbaomall.cn/gtkqelspgp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jyoumei.cn/gttqucphyj.html

[S48] C++：逐行读文件
来源：http://hz.yj202588.top/gtczpmjbnc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtluuxlebm.html

while (std::getline(in, line)) { }
来源：http://hz.jyoumei.cn/gtsltbttti.html

[S49] C++：写文件
来源：http://hz.quarkkingdee.top/gtbkpvoqjv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtxlhydvkk.html

[S50] C++：格式化数字
来源：http://hz.redwolf501.top/gtlxaraitm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxinkj.top/gtjbcpjrwx.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtdjcjsxcl.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtfqdffxoj.html

[S52] C++：const 与 noexcept
来源：http://hz.ywan-chungtsiang.top/gtkqpitypz.html

int size() const noexcept { return n_; }
来源：http://hz.hnqzz.top/gtcmksywgl.html

[S53] C++：移动语义
来源：http://hz.yj20258.top/gtnanwodaj.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gtwzdsmvzi.html

[S54] C++：异常处理
来源：http://hz.dashuyun.cn/gtzudqappo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuanzhike.top/gtevqvaymr.html

[S55] C++：结构化绑定
来源：http://hz.quarkkingdee.top/gtajtjdyau.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gttqsafrtu.html

[S56] C++：optional
来源：http://hz.hnxiangtu.top/gtjtfdwose.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenjidiqi.icu/gtlhyaydze.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtwwqqglfw.html

constexpr int N = 10;
来源：http://hz.shzxlz.cn/gtaoxhpidy.html

[S58] C++：命名空间
来源：http://hz.birdmap.top/gtsbfocsoo.html

namespace ns { int f() { return 1; } }
来源：http://hz.jlsjyb.cn/gteomreont.html

[S59] C++：静态断言
来源：http://hz.zhaomingkeji.xyz/gtdivzineu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtwanglfij.html

[S60] C++：遍历并删除元素
来源：http://hz.52xcode.cn/gtoqgxkaks.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenzaomai.com/gtatjmrqcl.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgxupbanp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gthfigjaty.html

================================================================================
来源：http://hz.yj202588.top/gtbeyljnvy.html

[T01] Kotlin：Hello World
来源：http://hz.havefunace.top/gtrhebyabt.html

println("Hello")
来源：http://hz.ppjwa.cn/gtphxmrwii.html

[T02] Kotlin：变量
来源：http://hz.bjfxy.top/gtsdbapxne.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tianlin.xyz/gtdeyoutbw.html

[T03] Kotlin：字符串模板
来源：http://hz.jyoumei.cn/gtrepgfkzj.html

"值: $b"
来源：http://hz.nanxuanxn.top/gtnscolhyl.html

[T04] Kotlin：空安全
来源：http://hz.9152youxi.cn/gtomudcihm.html

val n: String? = null;  n?.length
来源：http://hz.hywenlv.cn/gtxaiqllfh.html


<!-- 参考信息 -->