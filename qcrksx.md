代发 wailian999

name="${1:-default}"
来源：http://hz.feifeiyinyue.top/gtenpfgfpz.html

[R06] 判断命令是否存在
来源：http://hz.wangdashe.top/gtuxegjnzv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.svipenyu.cn/gtsisvopca.html

[R07] if 判断文件
来源：http://hz.xylfe.cn/gtdekwcdva.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zdqjudy.top/gtkuyjqnqc.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtbidhjazm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gttdygliqh.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gtvmqfuysy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.316326.xyz/gtzqawpcpv.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtzpmcowef.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtwzkfpvgr.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtcukemucx.html

case "$1" in
来源：http://hz.tanke756.top/gtbanrjnvk.html

start) echo "启动" ;;
来源：http://hz.haohaochexian.top/gtegpditcx.html

stop)  echo "停止" ;;
来源：http://hz.aizwys.cn/gthosymvxu.html

*)     echo "未知命令" ;;
来源：http://hz.nanxuanxn.top/gtucpaojjv.html

esac
来源：http://hz.sxryk.cn/gtwmgyromb.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtlfpnayet.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ppjwa.cn/gtrtdgugdz.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtdzlsbgwc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtalhxcaud.html

[R14] C 风格 for
来源：http://hz.hammf.cn/gtqhaopsgw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtomiabcjz.html

[R15] while 逐行读文件
来源：http://hz.iojbl.cn/gtfyvjfoth.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtughbucyf.html

[R16] until 等待条件
来源：http://hz.dianchejie.cn/gtldmntvey.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yongpay.top/gtaapauqlu.html

[R17] 数组定义与取值
来源：http://hz.hywenlv.cn/gtkibzpzsa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gtmdxwppaf.html

[R18] 遍历数组
来源：http://hz.jinyuanbaomall.cn/gtcnnfymlx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ywan-chungtsiang.top/gtpnxycrxl.html

[R19] 数组长度
来源：http://hz.nanxuanxn.top/gtqjstwfog.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtvotlmgip.html

[R20] 关联数组（字典）
来源：http://hz.wangshuangyany.cn/gtwqqvldoo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangshuangyany.cn/gtmodlrcqu.html

[R21] 字符串长度
来源：http://hz.aizwys.cn/gtqyldhvlv.html

echo "${#s}"
来源：http://hz.svipenyu.cn/gtqnlvyuxk.html

[R22] 截取子串
来源：http://hz.shuidangran.top/gtywswqzhz.html

echo "${s:0:5}"
来源：http://hz.yongpay.top/gtzqtawvkr.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtucxbjwno.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtzzorgwdj.html

[R24] 大小写转换
来源：http://hz.jqgufenzy.top/gtojudborx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuanzx.com/gtbsmmsnrf.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gtkufnkvdy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenzaomai.com/gtoiupukwy.html

[R26] 命令替换
来源：http://hz.shanyushiyangkeji.top/gtntoqvxck.html

now=$(date +%F); echo "$now"
来源：http://hz.meibo888.top/gtjatojteh.html

[R27] 算术展开
来源：http://hz.feifeiyinyue.top/gtbdssaxum.html

echo $((1 + 2 * 3))
来源：http://hz.chenzaomai.com/gtsndcfqpf.html

[R28] 浮点运算
来源：http://hz.yonumen.top/gteuivilnv.html

echo "scale=2; 10/3" | bc
来源：http://hz.0kj1m.cn/gtawphjrrv.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtoszslpxl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenzaomai.com/gtzvdelahe.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtnidkhswf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhoulong.xyz/gthtqmwukh.html

[R31] 局部变量
来源：http://hz.yj20258.top/gttosndtcj.html

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gtgfzohzhn.html

[R32] 参数个数校验
来源：http://hz.gogol.net.cn/gtszlgqftk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tianlin.xyz/gtjlliswrb.html

[R33] 捕获错误并提示行号
来源：http://hz.zycfv.cn/gtkriubulu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ehwqpu.com/gtsvtworbk.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtqcffwlbw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtvuicdnbs.html

[R35] 后台执行并等待
来源：http://hz.yuxming.cn/gtaypblimd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.smart0.xyz/gtinmlkzdd.html

[R36] 并发执行多个任务
来源：http://hz.tian-w.cn/gteicagqep.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hongshengwenyu.top/gtcirgdxkx.html

[R37] 把输出赋给变量
来源：http://hz.yj20258888.top/gtcgbyumes.html

files=$(ls -1)
来源：http://hz.birdmap.top/gttbukgtbk.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gtxmysbxhm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtrtomljwg.html

[R39] 重定向标准输出与错误
来源：http://hz.9152youxi.cn/gtbrcvgjcc.html

cmd > out.log 2>&1
来源：http://hz.birdmap.top/gtqgapuakz.html

[R40] 追加写日志
来源：http://hz.andypj.xyz/gtfcyriqeb.html

echo "log" >> out.log
来源：http://hz.shzxlz.cn/gtyvfdeesg.html

[R41] 丢弃输出
来源：http://hz.jqgfzy.top/gtlpnucuam.html

cmd >/dev/null 2>&1
来源：http://hz.tanke756.top/gtvttsrnst.html

[R42] 输入重定向
来源：http://hz.jinqigfzy.top/gtmumwdnzg.html

wc -l < a.txt
来源：http://hz.ywan-chungtsiang.top/gtoevdrbry.html

[R43] 按名字查找文件
来源：http://hz.zhongyouzk.top/gtwvzhdxjk.html

find . -name "*.log" -type f
来源：http://hz.hammf.cn/gtrsjrlnij.html

[R44] 按修改时间查找
来源：http://hz.andypj.xyz/gtnbwzhiay.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gtyaagfsse.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtartpmzys.html

find . -name "*.tmp" -delete
来源：http://hz.yuxming.cn/gtqpdzvrtq.html

[R46] 递归替换文件内容
来源：http://hz.xingfuxueyuan.xyz/gtnaftvzno.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gtdodkfbbc.html

[R47] sed 单行替换
来源：http://hz.guowangkeji.top/gtaeuetiob.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtwsrxdchl.html

[R48] awk 取指定列
来源：http://hz.zhixingplan.top/gtgyxdavwe.html

awk '{print $1, $3}' a.txt
来源：http://hz.havefunace.top/gtoacsyvbm.html

[R49] awk 带条件
来源：http://hz.0kj1m.cn/gtqxrasdah.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenzaomai.com/gtuqftlpki.html

[R50] awk 求和
来源：http://hz.shuidangran.top/gtrutvsptp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtbsevfxyi.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtrsnhrvud.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tanke756.top/gtogtujxxj.html

[R52] 统计行数
来源：http://hz.iojbl.cn/gtxxgxhugn.html

wc -l a.txt
来源：http://hz.nanxinkj.top/gttianpfuu.html

[R53] 查看文件头与实时尾
来源：http://hz.birdmap.top/gteiigdzzv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtizyxbxyk.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gtgynxvtme.html

diff a.txt b.txt
来源：http://hz.yuanzhike.top/gtyypymypf.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtzqclfkuh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydzc1.top/gtdtkyrlmh.html

[R56] 远程拷贝
来源：http://hz.daria6918.cn/gtiwwldlmn.html

scp file user@host:/path/
来源：http://hz.xylfe.cn/gtbhjgoeum.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtjdljdsig.html

ssh user@host 'uptime'
来源：http://hz.cheryme.top/gtqvmacffu.html

[R58] 下载文件
来源：http://hz.hnxiangtu.top/gtgkklzman.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydzc1.top/gtgprlmmsa.html

[R59] 发 POST JSON
来源：http://hz.redwolf501.top/gtqfivbawz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gthmvkzekd.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxuanxn.top/gttkcwehcd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinyuanbaomall.cn/gtnqdphqmw.html

[R61] 磁盘占用
来源：http://hz.cashguo.top/gtcpbtjyxn.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gthnujvmoa.html

[R62] 找最占空间的文件
来源：http://hz.52xcode.cn/gtedaorflj.html

du -ah . | sort -rh | head -10
来源：http://hz.sufxvd.cn/gtaojkquat.html

[R63] 内存与进程
来源：http://hz.xylfe.cn/gtvadeloae.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtuiaemunw.html

[R64] 结束进程
来源：http://hz.ywan-chungtsiang.top/gtscfnpguj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sweek.top/gtkbannpxu.html

[R65] 查看端口占用
来源：http://hz.xziqi.cn/gtvrpqqepc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.svipenyu.cn/gtmnuohlvu.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtipxcqrua.html

crontab -e;  crontab -l
来源：http://hz.gotoacloud.top/gtnntxaypj.html

[R67] 生成随机十六进制串
来源：http://hz.fengsongda.top/gtqsrikkyr.html

openssl rand -hex 16
来源：http://hz.jinyuanbaomall.cn/gtmrwavaps.html

[R68] 计算文件校验值
来源：http://hz.hysaishi.cn/gtpdltkwqb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtvcmxjlss.html

[R69] 生成随机密码
来源：http://hz.chenlongwang.top/gtopzwbpmz.html

head -c 16 /dev/urandom | base64
来源：http://hz.meibo888.top/gtgtuqggco.html

[R70] 时间戳与互转
来源：http://hz.jiagoushi.top/gtfggggygu.html

date +%s;  date -d @1700000000
来源：http://hz.tanke756.top/gtgurrtwwm.html

[R71] 日期格式化
来源：http://hz.dashuyun.cn/gthoullryw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtdlctkocn.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gthehdctgl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.havefunace.top/gtxezvesmg.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtlbkrxhzf.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtnforqxje.html

[R74] 批量重命名
来源：http://hz.yj20258.top/gtvggjuida.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtejzugcvq.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gtshbzbvpe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hfpthk.cn/gtggkocyrg.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtjnpqqvne.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtmhxmwigy.html

[R77] 读取用户输入
来源：http://hz.snrcjt.cn/gtuvygaiqf.html

read -rp "请输入: " ans
来源：http://hz.wangshuangyany.cn/gtpvyedbpi.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gtmivivfjb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hywenlv.cn/gtikhyhaew.html

[R79] 解析命令行选项
来源：http://hz.cheryme.top/gtdgzuigpu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.0kj1m.cn/gtxwikxvzo.html

[R80] 查看脚本执行耗时
来源：http://hz.chenlongwang.top/gtqadzdoqa.html

time ./run.sh
来源：http://hz.svipenyu.cn/gtrmfxxkbd.html

================================================================================
来源：http://hz.gzhubu.top/gtsubcfjwj.html

S. C / C++ 专题
来源：http://hz.tanke756.top/gtpiprqioe.html

================================================================================
来源：http://hz.xziqi.cn/gtzfvedzcp.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gtktjewshc.html

#include <stdio.h>
来源：http://hz.ydzc1.top/gtpbqdudsa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jiagoushi.top/gtwtspksyb.html

[S02] C：变量与格式化输出
来源：http://hz.fzhhl.top/gtvljpwayb.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtomxzyqdq.html

[S03] C：读入整数
来源：http://hz.sufxvd.cn/gtkguegiuu.html

int x; scanf("%d", &x);
来源：http://hz.cucudq.cn/gtattqigqj.html

[S04] C：字符串复制
来源：http://hz.chenzaomai.com/gtorqjrcon.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.c1oappe.top/gttgbtyjrh.html

[S05] C：字符串长度
来源：http://hz.cashguo.top/gtytyebdez.html

strlen(s)
来源：http://hz.quarkkingdee.top/gtgpugkmms.html

[S06] C：字符串比较
来源：http://hz.cashguo.top/gtsgufzuon.html

strcmp(a, b) == 0
来源：http://hz.pengpengdd.cyou/gtmhuheajt.html

[S07] C：数组遍历求和
来源：http://hz.xuanzx.com/gtjbanlixv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinyuanbaomall.cn/gtofwidpih.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gtifrsznir.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258888.top/gtjytplnhj.html

[S09] C：结构体定义与初始化
来源：http://hz.andypj.xyz/gtppthiawd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cheryme.top/gttmfmdvln.html

[S10] C：指针与解引用
来源：http://hz.jianghu66.top/gtkfyeoego.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtmnfhxgfq.html

[S11] C：逐行读文件
来源：http://hz.nwbrower.top/gtriltibmn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shanyushiyangkeji.top/gtluobynru.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ywan-chungtsiang.top/gtjroznykj.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtcarkbdia.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtyintixsi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sufxvd.cn/gtvthmsywj.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtthsobllt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shangyingyoupin.top/gtznbajicy.html

[S14] C：枚举
来源：http://hz.hammf.cn/gtbmesxuhc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gthdhtkuey.html

[S15] C：类型转换
来源：http://hz.zdqjudy.top/gtgrhmqwus.html

(double) a / b
来源：http://hz.haohaochexian.top/gtyufnmeoi.html

[S16] C：位操作置位
来源：http://hz.jyoumei.cn/gtnbdnnyyz.html

x |= (1 << 3);
来源：http://hz.yonumen.top/gtxfdhewnu.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtljsudmtf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtwlmxbdon.html

[S18] C：命令行参数
来源：http://hz.c1oappe.top/gtpifdryvh.html

int main(int argc, char **argv)
来源：http://hz.zhijiandao.cn/gtgllehgvp.html

[S19] C：快速排序
来源：http://hz.xinyue.icu/gtwmcgemlg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtvqjkbmgv.html

[S20] C：二分查找
来源：http://hz.jinyuanbaomall.cn/gtfhujokee.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtellndfhs.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtziftunml.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtqqalpqzq.html

[S22] C：字符串转数字
来源：http://hz.cqqwz.cn/gtxwneakct.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gtonuojjvw.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtkyolptsz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.redwolf501.top/gtmlafjbds.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtjdyhaxmh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhixingplan.top/gtiroypqjq.html

[S25] C：内存拷贝
来源：http://hz.redwolf501.top/gtcrajgjtq.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtymnkbjtq.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gthyrxocjt.html

memset(a, 0, sizeof a);
来源：http://hz.yanxiufei.cn/gtwbwbiqux.html

[S27] C：定义常量
来源：http://hz.shanyushiyangkeji.top/gtkgviukra.html

const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtegzehknq.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gtaglmhimv.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gtqjrvlvye.html

[S29] C：变参函数
来源：http://hz.jinghuilouyu.cn/gtiyhyvtgf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhijiandao.cn/gttgcwebgr.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtrbpsjsua.html

#ifndef X_H
来源：http://hz.yj202588.top/gtfooifvgs.html

#define X_H
来源：http://hz.sxryk.cn/gtpbnbzyoh.html

#endif
来源：http://hz.xinyue.icu/gtubejqtqi.html

[S31] C++：Hello World
来源：http://hz.cheryme.top/gtmvbvzhoe.html

#include <iostream>
来源：http://hz.cucudq.cn/gtydelgyua.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtfkrmjsor.html

[S32] C++：字符串
来源：http://hz.quarkkingdee.top/gtjwxwyhss.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigfzy.top/gtwlmcvnis.html

[S33] C++：vector 增删
来源：http://hz.daxiang520.top/gtkwlrlttq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xuetiantiany.cn/gtfaalxiud.html

[S34] C++：遍历 vector
来源：http://hz.jinqigufen.top/gtwzpzbxwc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zycfv.cn/gtgrhfcnox.html

[S35] C++：map
来源：http://hz.xylfe.cn/gtpaepzqoc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangtech.top/gtwveujcof.html

[S36] C++：unordered_map
来源：http://hz.aibaodan.cn/gtueqxequc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtckxpptwb.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtacvjbzpi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.svipenyu.cn/gtnsnirbdz.html

[S38] C++：排序
来源：http://hz.shuidangran.top/gtjzgncjwy.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtydfuhtjm.html

[S39] C++：自定义比较器排序
来源：http://hz.316326.xyz/gtpguqagof.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtlqvnnoqf.html

[S40] C++：查找元素
来源：http://hz.hnxiangtu.top/gtbfpifypl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jiagoushi.top/gtumoufzqv.html

[S41] C++：类与构造函数
来源：http://hz.jinqigufen.top/gtxocujjsn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ywan-chungtsiang.top/gttczcyluk.html

[S42] C++：继承与虚函数
来源：http://hz.shangyingyoupin.top/gtirrnxgek.html

class B : public Base { public: void f() override {} };
来源：http://hz.gaohongyu789.top/gtxwhtgvdh.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtxycckiig.html

auto p = std::make_unique<int>(5);
来源：http://hz.redwolf501.top/gtiquxaoem.html

[S44] C++：引用传参
来源：http://hz.tianlin.xyz/gtahvoeaab.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gtnggohegf.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtkhbbmuwx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigfzy.top/gthyuhewkz.html

[S46] C++：函数模板
来源：http://hz.hnxiangtu.top/gtewstvmjm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangshuangyany.cn/gtyskffaxq.html

[S47] C++：结构化绑定遍历
来源：http://hz.quarkkingdee.top/gtmqjgwnmm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gtuvxvegns.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtsumlrmol.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xinyue.icu/gtwjnksfaq.html

while (std::getline(in, line)) { }
来源：http://hz.sweek.top/gtadbgojjw.html

[S49] C++：写文件
来源：http://hz.snrcjt.cn/gtegomitdf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jiagoushi.top/gtnuqiaiii.html

[S50] C++：格式化数字
来源：http://hz.52xcode.cn/gthshozlpd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258.top/gtcbyswamf.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtlcllaxzb.html

static_cast<double>(a) / b
来源：http://hz.cucudq.cn/gtewcgvpgp.html

[S52] C++：const 与 noexcept
来源：http://hz.hnqzz.top/gtuonffrdq.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gtpeksmifj.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtsgxkzzxa.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtsewdezqy.html

[S54] C++：异常处理
来源：http://hz.xuanzx.com/gttpbqcotg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtzkyftizx.html

[S55] C++：结构化绑定
来源：http://hz.mhx1999.top/gtodjyuuus.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhongyouzk.top/gttmjevdbp.html

[S56] C++：optional
来源：http://hz.bjfxy.top/gtudjqzzwz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydjk.org.cn/gtjdozexfs.html

[S57] C++：编译期常量
来源：http://hz.yueranfly.top/gtvqfigbwo.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtaemvumvw.html

[S58] C++：命名空间
来源：http://hz.feifeiyinyue.top/gtaueaegzx.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxuanxn.top/gtpmflszdm.html

[S59] C++：静态断言
来源：http://hz.daria6918.cn/gturjhwvgu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhoulong.xyz/gtibguyhyj.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigfzy.top/gtotcecqse.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxuanxn.top/gtnlqgxhnc.html

================================================================================
来源：http://hz.ybcxt.top/gtwiuidenz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtoviturqg.html

================================================================================
来源：http://hz.zdqjudy.top/gtxcbgmiuw.html

[T01] Kotlin：Hello World
来源：http://hz.shuidangran.top/gtsrgcxban.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtzlhcjemf.html

[T02] Kotlin：变量
来源：http://hz.nwbrower.top/gtohhbmfxp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnxiangtu.top/gtcparruhy.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtstqrxova.html

"值: $b"
来源：http://hz.snrcjt.cn/gttewqrvkq.html

[T04] Kotlin：空安全
来源：http://hz.ehwqpu.com/gtgfkyxqrp.html

val n: String? = null;  n?.length
来源：http://hz.sxryk.cn/gthbqvhgge.html

[T05] Kotlin：when 表达式
来源：http://hz.xuetiantiany.cn/gtbocqzynn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ivvv.top/gtyuowqehs.html

[T06] Kotlin：集合映射
来源：http://hz.zhiwuduotai.top/gthkuujvyw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtadxwtrwv.html


<!-- 参考信息 -->