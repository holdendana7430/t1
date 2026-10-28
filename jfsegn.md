代发 wailian999

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtjjbxlqkd.html

[R06] 判断命令是否存在
来源：http://hz.xziqi.cn/gtvzmjzsdb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuanzx.com/gtrojkyijo.html

[R07] if 判断文件
来源：http://hz.zhaomingkeji.xyz/gtpcxemnul.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtjvsoclxj.html

[R08] 数值比较
来源：http://hz.jinqigufen.top/gttkcqkzbi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinqigufen.top/gtkohpwlqh.html

[R09] 字符串比较
来源：http://hz.hnxiangtu.top/gtcwvhoaia.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtceydsgxu.html

[R10] 正则匹配
来源：http://hz.jinghuilouyu.cn/gtlztuygvn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.snrcjt.cn/gtjspqgcgw.html

[R11] case 多分支
来源：http://hz.zdqjudy.top/gtwxqiqvmq.html

case "$1" in
来源：http://hz.hfpthk.cn/gtgjxwoggu.html

start) echo "启动" ;;
来源：http://hz.jlsjyb.cn/gtvhlvushz.html

stop)  echo "停止" ;;
来源：http://hz.hnxiangtu.top/gtknqzertv.html

*)     echo "未知命令" ;;
来源：http://hz.haohaochexian.top/gtysmwzffi.html

esac
来源：http://hz.hywenlv.cn/gtqtdtlhrq.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtmpxlrbss.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhiwuduotai.top/gtyzeysmgw.html

[R13] for 计数循环
来源：http://hz.nwbrower.top/gtdqehozyo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shuidangran.top/gteziiyhkr.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gtjjkdxggt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gtzyxohxgf.html

[R15] while 逐行读文件
来源：http://hz.havefunace.top/gtcrxkwcwx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhixingplan.top/gtpwxignoq.html

[R16] until 等待条件
来源：http://hz.9152youxi.cn/gtvosmejgj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangshuangyany.cn/gtlfkvxlkp.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangkeji.top/gtrjmwgihi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gotoacloud.top/gtajehxhia.html

[R18] 遍历数组
来源：http://hz.pycfn.com/gtbkinvhoh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.pengpengdd.cyou/gtnrkvoahs.html

[R19] 数组长度
来源：http://hz.jinqigfzy.top/gtpoktkwbn.html

echo "${#arr[@]}"
来源：http://hz.jiagoushi.top/gtnupzizyp.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gtdbdxublu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtidwgswtc.html

[R21] 字符串长度
来源：http://hz.redwolf501.top/gtktqlpuav.html

echo "${#s}"
来源：http://hz.ybcxt.top/gtjcahzizm.html

[R22] 截取子串
来源：http://hz.gotoacloud.top/gtonzcgztr.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtufnkdavh.html

[R23] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gtczgdhogx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenzaomai.com/gtswkueusz.html

[R24] 大小写转换
来源：http://hz.mhx1999.top/gtwzmbqpth.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.kuanghao11.cn/gtcjcxunbo.html

[R25] 去后缀 / 去前缀
来源：http://hz.sxryk.cn/gtdnicvxlh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cheryme.top/gtanpbcxek.html

[R26] 命令替换
来源：http://hz.yanxiufei.cn/gtzzwonksl.html

now=$(date +%F); echo "$now"
来源：http://hz.52xcode.cn/gtioqjegtg.html

[R27] 算术展开
来源：http://hz.sweek.top/gtcsksvpyd.html

echo $((1 + 2 * 3))
来源：http://hz.redwolf501.top/gtvytcwtqn.html

[R28] 浮点运算
来源：http://hz.zhaomingkeji.xyz/gttnctcahw.html

echo "scale=2; 10/3" | bc
来源：http://hz.dashuyun.cn/gtwdfrecwr.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtlovybthy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gtgzswfmrq.html

[R30] 函数返回状态码
来源：http://hz.sufxvd.cn/gtqlcaxoke.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nwbrower.top/gtswawudkb.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gthvxlgkhd.html

f() { local x=1; echo "$x"; }
来源：http://hz.xingfuxueyuan.xyz/gtmmfmgheq.html

[R32] 参数个数校验
来源：http://hz.yongpay.top/gtexeomrov.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gthoeicocw.html

[R33] 捕获错误并提示行号
来源：http://hz.daria6918.cn/gtsolvknjx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gotoacloud.top/gtvacwvmjj.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gtpubzemqf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtylmmmqke.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtwdponols.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.haohaochexian.top/gtoyzfwhgk.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtczjnoxfy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinqigfzy.top/gtpoxbwlze.html

[R37] 把输出赋给变量
来源：http://hz.smart0.xyz/gtnyvzwypw.html

files=$(ls -1)
来源：http://hz.zhoulong.xyz/gtmtzccrfz.html

[R38] 管道串联
来源：http://hz.birdmap.top/gtpqgwanee.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtapdaccac.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtyqhqnena.html

cmd > out.log 2>&1
来源：http://hz.jinyuanbaomall.cn/gtlkwokqph.html

[R40] 追加写日志
来源：http://hz.quarkkingdee.top/gtjcykyjpj.html

echo "log" >> out.log
来源：http://hz.zhixingplan.top/gtljwuwssw.html

[R41] 丢弃输出
来源：http://hz.snrcjt.cn/gtovrcqifj.html

cmd >/dev/null 2>&1
来源：http://hz.ybcxt.top/gtrmdyzvoq.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtoyeqnbzc.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtqujmdjvh.html

[R43] 按名字查找文件
来源：http://hz.jianghu66.top/gttfctkvoc.html

find . -name "*.log" -type f
来源：http://hz.feifeiyinyue.top/gtwaacsfcy.html

[R44] 按修改时间查找
来源：http://hz.ybcxt.top/gtyjywkpht.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtspkpslwu.html

[R45] 批量删除
来源：http://hz.gzhubu.top/gtnujsound.html

find . -name "*.tmp" -delete
来源：http://hz.ehwqpu.com/gtvjievkxk.html

[R46] 递归替换文件内容
来源：http://hz.nanxuanxn.top/gtiqqxfxgs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tian-w.cn/gtgolccztv.html

[R47] sed 单行替换
来源：http://hz.hnxiangtu.top/gttyduuslu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtaenpqvqs.html

[R48] awk 取指定列
来源：http://hz.zhoulong.xyz/gtxlcshozi.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258.top/gtvinvhued.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtadpxsyjp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ehwqpu.com/gtpsajljfn.html

[R50] awk 求和
来源：http://hz.sufxvd.cn/gtfegrdfsa.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gtwcyzdhqs.html

[R51] 排序去重取前几
来源：http://hz.yj20258.top/gtkaoabyho.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dashuyun.cn/gtxevuxtap.html

[R52] 统计行数
来源：http://hz.zdqjudy.top/gtpbetdccm.html

wc -l a.txt
来源：http://hz.zhaomingkeji.xyz/gtbknjrsdd.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtthkrpwix.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.quarkkingdee.top/gtpcrfpkzy.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtucsfnzsm.html

diff a.txt b.txt
来源：http://hz.vqdsnc.cn/gtjlgcnvkp.html

[R55] 压缩与解压
来源：http://hz.wangdashe.top/gtdcbabpnh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtodmvpijv.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangtech.top/gtnlafmpys.html

scp file user@host:/path/
来源：http://hz.gogol.net.cn/gtwrlxkqxm.html

[R57] 远程执行命令
来源：http://hz.fengsongda.top/gtbmmyfcdw.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtqzlmexfd.html

[R58] 下载文件
来源：http://hz.andypj.xyz/gtkegicrml.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gtvgdpgkyw.html

[R59] 发 POST JSON
来源：http://hz.xuetiantiany.cn/gthoxryovn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gttxqlcwer.html

[R60] 只看 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtxlhpotks.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tanke756.top/gtlwdizljr.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtzdoetncd.html

df -h;  du -sh *
来源：http://hz.hnxiangtu.top/gtfdxbbpwn.html

[R62] 找最占空间的文件
来源：http://hz.yueranfly.top/gtywjryyyp.html

du -ah . | sort -rh | head -10
来源：http://hz.meibo888.top/gtjcpiykub.html

[R63] 内存与进程
来源：http://hz.hysaishi.cn/gtstcdmfyf.html

free -h;  ps aux | grep nginx
来源：http://hz.fengsongda.top/gtdzhixiui.html

[R64] 结束进程
来源：http://hz.ivvv.top/gtsfwcljds.html

kill -9 $(pgrep -f app.py)
来源：http://hz.vqdsnc.cn/gtwxqwcoir.html

[R65] 查看端口占用
来源：http://hz.xziqi.cn/gtmbdicfwo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gterdkidrm.html

[R66] 定时任务
来源：http://hz.shanyushiyangtech.top/gtkmabljwu.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtavbbyhkd.html

[R67] 生成随机十六进制串
来源：http://hz.hnqzz.top/gtjquyxyaf.html

openssl rand -hex 16
来源：http://hz.hnqzz.top/gtxyyhvkkg.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtlrjwfhpm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ybcxt.top/gtwzetuorl.html

[R69] 生成随机密码
来源：http://hz.yuxming.cn/gtzryqtmum.html

head -c 16 /dev/urandom | base64
来源：http://hz.dashuyun.cn/gtevwfthfi.html

[R70] 时间戳与互转
来源：http://hz.xylfe.cn/gtioudflid.html

date +%s;  date -d @1700000000
来源：http://hz.nwbrower.top/gtmymkiaob.html

[R71] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtxlcaykqk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daria6918.cn/gtfdrairut.html

[R72] 等待端口就绪
来源：http://hz.nanxinkj.top/gtxmekxfup.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gtexiykaix.html

[R73] 分割大日志
来源：http://hz.vqdsnc.cn/gtanweowxt.html

split -l 1000 big.log part_
来源：http://hz.yuxming.cn/gtxcxbsdzk.html

[R74] 批量重命名
来源：http://hz.shanyushiyangtech.top/gtdbdgzbqu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhijiandao.cn/gtsiekssxz.html

[R75] 导出环境变量
来源：http://hz.ybcxt.top/gtmuamkvqd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dashuyun.cn/gtjlbrveqk.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gtqhvbtaib.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtvijmvzpg.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtelgvcpmw.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtibsrrepo.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtifsccgzx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ppjwa.cn/gtuortqpwp.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtzpolghcd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gogol.net.cn/gtthkoerfb.html

[R80] 查看脚本执行耗时
来源：http://hz.yongpay.top/gtckvgzzbx.html

time ./run.sh
来源：http://hz.yongpay.top/gtqqdkdbmw.html

================================================================================
来源：http://hz.nwbrower.top/gtdixgstcs.html

S. C / C++ 专题
来源：http://hz.guowangkeji.top/gtbzcqvpwg.html

================================================================================
来源：http://hz.zhixingplan.top/gtaogibazs.html

[S01] C：Hello World
来源：http://hz.quarkkingdee.top/gtbzchcbhj.html

#include <stdio.h>
来源：http://hz.jiagoushi.top/gtqnjwhxrh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.c1oappe.top/gtgwzezsve.html

[S02] C：变量与格式化输出
来源：http://hz.chenlongwang.top/gtnmxhzhrm.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtvnmrnoot.html

[S03] C：读入整数
来源：http://hz.jinghuilouyu.cn/gtmchcchir.html

int x; scanf("%d", &x);
来源：http://hz.cheryme.top/gtndlbqsht.html

[S04] C：字符串复制
来源：http://hz.yongpay.top/gtheyahtjs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtyxszqnpr.html

[S05] C：字符串长度
来源：http://hz.tanke756.top/gtqoekntlm.html

strlen(s)
来源：http://hz.yvedp.cn/gtknbesaor.html

[S06] C：字符串比较
来源：http://hz.dashuyun.cn/gtolekeoqe.html

strcmp(a, b) == 0
来源：http://hz.jinyuanbaomall.cn/gtajxdjtjz.html

[S07] C：数组遍历求和
来源：http://hz.yvedp.cn/gtgdsmnhez.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtokchvjqx.html

[S08] C：动态内存分配与释放
来源：http://hz.c1oappe.top/gtrvuydout.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fzhhl.top/gttqtysulw.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gtrnutzkjy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhijiandao.cn/gteenylkcc.html

[S10] C：指针与解引用
来源：http://hz.pycfn.com/gtgprwsxvf.html

int *p = &a;  *p = 5;
来源：http://hz.gogol.net.cn/gtcvfqxotv.html

[S11] C：逐行读文件
来源：http://hz.iojbl.cn/gtwftmnuyh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtibgieciz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhixingplan.top/gtvwjctjxg.html

fclose(f);
来源：http://hz.jyoumei.cn/gthxnownpk.html

[S12] C：写文件
来源：http://hz.ybcxt.top/gtxyjnryxb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.havefunace.top/gttvcbmmda.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtyuotkene.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gotoacloud.top/gteoqcestz.html

[S14] C：枚举
来源：http://hz.shanyushiyangkeji.top/gtvnoguhgh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.haohaochexian.top/gtjdmaunzk.html

[S15] C：类型转换
来源：http://hz.jqgfzy.top/gtjofzxgux.html

(double) a / b
来源：http://hz.gzhubu.top/gtzvxhggpq.html

[S16] C：位操作置位
来源：http://hz.sxryk.cn/gtqezmwgvz.html

x |= (1 << 3);
来源：http://hz.pengpengdd.cyou/gtkdsdlfbb.html

[S17] C：安全拼接字符串
来源：http://hz.feifeiyinyue.top/gtlznvkpke.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenlongwang.top/gttrmazzid.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtaoykoukx.html

int main(int argc, char **argv)
来源：http://hz.ivvv.top/gtzhbqwgwo.html

[S19] C：快速排序
来源：http://hz.svipenyu.cn/gtgqyinern.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtuowjhuay.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gtwbheimxk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtgkwdhrsp.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangkeji.top/gthymygymq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.birdmap.top/gtwtryjqcm.html

[S22] C：字符串转数字
来源：http://hz.hnxiangtu.top/gtvdxbguph.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shangyingyoupin.top/gthznlwptu.html

[S23] C：随机数
来源：http://hz.jiagoushi.top/gthteteode.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnqzz.top/gteiroawez.html

[S24] C：获取本地时间
来源：http://hz.zycfv.cn/gtuuxjtjql.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.havefunace.top/gtgqwbptik.html

[S25] C：内存拷贝
来源：http://hz.hfpthk.cn/gtziyglfxo.html

memcpy(dst, src, n);
来源：http://hz.hnxiangtu.top/gtwyxxyvhb.html

[S26] C：内存清零
来源：http://hz.xuanzx.com/gtrrhpcfju.html

memset(a, 0, sizeof a);
来源：http://hz.jqgfzy.top/gtdmkznlzs.html

[S27] C：定义常量
来源：http://hz.xuanzx.com/gtsgtnsaqm.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtwroeetpg.html

[S28] C：静态变量
来源：http://hz.snrcjt.cn/gtrhkmsndp.html

static int counter = 0;
来源：http://hz.aibaodan.cn/gtafynugvg.html

[S29] C：变参函数
来源：http://hz.chenzaomai.com/gtvawvljqn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.c1oappe.top/gtnznomrbi.html

[S30] C：头文件保护
来源：http://hz.ywan-chungtsiang.top/gttwhyueon.html

#ifndef X_H
来源：http://hz.jinghuilouyu.cn/gtozhkevge.html

#define X_H
来源：http://hz.jiagoushi.top/gteadxwjmi.html

#endif
来源：http://hz.ppjwa.cn/gtjuggsxrz.html

[S31] C++：Hello World
来源：http://hz.iojbl.cn/gtilkitlws.html

#include <iostream>
来源：http://hz.yj202588.top/gtgdaegfrk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cqqwz.cn/gtlunnrwlp.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtzlllmglc.html

std::string s = "hi";  s += "!";
来源：http://hz.ivvv.top/gtfsmqzajx.html

[S33] C++：vector 增删
来源：http://hz.ppjwa.cn/gtpwyfwgba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenjidiqi.icu/gtbxbfyigh.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtxxjfirwc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gtyobgcgop.html

[S35] C++：map
来源：http://hz.zhaomingkeji.xyz/gtwakevfrz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtcahfrbss.html

[S36] C++：unordered_map
来源：http://hz.jinyuanbaomall.cn/gtvvqliwha.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtuurgpalt.html

[S37] C++：set
来源：http://hz.jqgfzy.top/gtmtpqcrib.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinghuilouyu.cn/gtzljihnik.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtzpkxjipq.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtkzktibow.html

[S39] C++：自定义比较器排序
来源：http://hz.guannengcc.top/gteorqodbg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258888.top/gtwzdamkwu.html

[S40] C++：查找元素
来源：http://hz.haohaochexian.top/gtrmbqlehs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.iojbl.cn/gtcufxpxmo.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangkeji.top/gtwzywmzqz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigufen.top/gttfwtbqmk.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gttjvecprm.html

class B : public Base { public: void f() override {} };
来源：http://hz.smart0.xyz/gtcxcsoetj.html

[S43] C++：智能指针
来源：http://hz.daria6918.cn/gtgpjypjrq.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenzaomai.com/gtonkvtgdj.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gtavgvclwk.html

void inc(int &x) { ++x; }
来源：http://hz.hysaishi.cn/gtcysjeciq.html

[S45] C++：lambda
来源：http://hz.ybcxt.top/gtdudhyspl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtstrviprw.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtpljuvgjv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydzc1.top/gtxlymmgwk.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangshuangyany.cn/gtckcwezol.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.iojbl.cn/gthoinycju.html

[S48] C++：逐行读文件
来源：http://hz.gogol.net.cn/gtqyxcrqqz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shangyingyoupin.top/gtthycrbqb.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gtgdxqahym.html

[S49] C++：写文件
来源：http://hz.shuidangran.top/gtssecgdhn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cashguo.top/gtqndukxef.html

[S50] C++：格式化数字
来源：http://hz.daxiang520.top/gtrjbnadfg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtmebeclue.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtzqrufunp.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtqzxvrrzw.html

[S52] C++：const 与 noexcept
来源：http://hz.hywenlv.cn/gtykmoqkrk.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gtfcgeebxu.html

[S53] C++：移动语义
来源：http://hz.zhoulong.xyz/gtisuwiemb.html

std::vector<int> w = std::move(v);
来源：http://hz.ydjk.org.cn/gtnimqlupo.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gtrqcrwqaj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ehwqpu.com/gtqvmkxena.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtkrbsalwe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cucudq.cn/gtbjvpxnbm.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gtkddefktc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtilqrdqpu.html

[S57] C++：编译期常量
来源：http://hz.zdqjudy.top/gtvlvrwqmv.html

constexpr int N = 10;
来源：http://hz.yanxiufei.cn/gtcynwmgui.html

[S58] C++：命名空间
来源：http://hz.ppjwa.cn/gtdsyhkugv.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258.top/gtkntdwtax.html

[S59] C++：静态断言
来源：http://hz.c1oappe.top/gtusnrzasl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yongpay.top/gtqvxhpzwy.html

[S60] C++：遍历并删除元素
来源：http://hz.tianlin.xyz/gtueykzvjx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtmyhohyfi.html

================================================================================
来源：http://hz.sysykeji.top/gtvndinadj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigfzy.top/gtcjlrpsfq.html

================================================================================
来源：http://hz.ybcxt.top/gtqacsppdn.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtlhqtalmi.html

println("Hello")
来源：http://hz.daria6918.cn/gtqblkvdgd.html

[T02] Kotlin：变量
来源：http://hz.fzhhl.top/gtqnpmpbdu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenlongwang.top/gtstoufoxx.html

[T03] Kotlin：字符串模板
来源：http://hz.yuanzhike.top/gtbnpouhrm.html

"值: $b"
来源：http://hz.aibaodan.cn/gtcbfqroos.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gtkacbvfzz.html

val n: String? = null;  n?.length
来源：http://hz.wangdashe.top/gthvinulta.html

[T05] Kotlin：when 表达式
来源：http://hz.xziqi.cn/gtdgfyrkix.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.9152youxi.cn/gtzjuvnasd.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gttcanults.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sweek.top/gtllbcvhbr.html


<!-- 参考信息 -->