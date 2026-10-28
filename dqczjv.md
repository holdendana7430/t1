代发 wailian999

R. Bash 专题
来源：http://hz.nanxuanxn.top/gtdrgwhfwq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtseitrzms.html

[R01] shebang 与严格模式
来源：http://hz.tianlin.xyz/gtumkmkeew.html

#!/usr/bin/env bash
来源：http://hz.ehwqpu.com/gtrwjwdzns.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gtfotbinbl.html

[R02] 变量赋值与使用
来源：http://hz.shangyingyoupin.top/gtwjdreuyd.html

name="Tom"; echo "$name"
来源：http://hz.xziqi.cn/gtxkmdiuuk.html

[R03] 只读变量
来源：http://hz.tian-w.cn/gtayjotpyr.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gttynzeciy.html

[R04] 位置参数
来源：http://hz.chenzaomai.com/gttcrpsiau.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nwbrower.top/gtzbwlxoog.html

[R05] 参数默认值
来源：http://hz.chenjidiqi.icu/gtkqfghtvr.html

name="${1:-default}"
来源：http://hz.ywan-chungtsiang.top/gtwxdtjmbi.html

[R06] 判断命令是否存在
来源：http://hz.yangfankeji.com/gtooejcklw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenzaomai.com/gtctebcnyu.html

[R07] if 判断文件
来源：http://hz.hongshengwenyu.top/gttdujaetw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.c1oappe.top/gtemrrcdzo.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtijdosrcl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtgctklhch.html

[R09] 字符串比较
来源：http://hz.pycfn.com/gtlchqrocp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.shangyingyoupin.top/gtbfcqjpci.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtyocuihfc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtsoparbms.html

[R11] case 多分支
来源：http://hz.hammf.cn/gtwaxfzgui.html

case "$1" in
来源：http://hz.smart0.xyz/gtsikoqcdh.html

start) echo "启动" ;;
来源：http://hz.hnxiangtu.top/gtvpkmyojl.html

stop)  echo "停止" ;;
来源：http://hz.andypj.xyz/gtwsaceums.html

*)     echo "未知命令" ;;
来源：http://hz.zhaomingkeji.xyz/gtsipuojyj.html

esac
来源：http://hz.ydjk.org.cn/gtczhazlbc.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtnohqcmzj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gotoacloud.top/gtggbbaeww.html

[R13] for 计数循环
来源：http://hz.nanxinkj.top/gtslmdihhv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhaomingkeji.xyz/gtdyqfklpc.html

[R14] C 风格 for
来源：http://hz.316326.xyz/gtgbvynhsj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gtpkvydzof.html

[R15] while 逐行读文件
来源：http://hz.c1oappe.top/gtclvlnteq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jiagoushi.top/gtpnxrwpmq.html

[R16] until 等待条件
来源：http://hz.xziqi.cn/gtpcmyoscl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gtsgivngoi.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtsheawyns.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.snrcjt.cn/gtkyvmohah.html

[R18] 遍历数组
来源：http://hz.cheryme.top/gtojvynwgk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenzaomai.com/gtwahcfwqj.html

[R19] 数组长度
来源：http://hz.hammf.cn/gtovmdagmj.html

echo "${#arr[@]}"
来源：http://hz.ivvv.top/gtxqztdcez.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtadphjzpa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ehwqpu.com/gtqfehmndq.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gtlbjrbzpo.html

echo "${#s}"
来源：http://hz.dianchejie.cn/gteiyuoxmv.html

[R22] 截取子串
来源：http://hz.shanyushiyangkeji.top/gtjwzivlgp.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtijaawgmn.html

[R23] 字符串替换
来源：http://hz.xuanzx.com/gtzsvlzgth.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.iojbl.cn/gtyzxlkkze.html

[R24] 大小写转换
来源：http://hz.hfpthk.cn/gtjyrrjyfs.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj202588.top/gthtrmdcmw.html

[R25] 去后缀 / 去前缀
来源：http://hz.gotoacloud.top/gttrhmabnl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sysykeji.top/gtoahiawtn.html

[R26] 命令替换
来源：http://hz.cqqwz.cn/gtybhypgbs.html

now=$(date +%F); echo "$now"
来源：http://hz.ybcxt.top/gtyosntcdt.html

[R27] 算术展开
来源：http://hz.tian-w.cn/gtplfjzwud.html

echo $((1 + 2 * 3))
来源：http://hz.9152youxi.cn/gtveexmhvb.html

[R28] 浮点运算
来源：http://hz.iojbl.cn/gtowjmwjxk.html

echo "scale=2; 10/3" | bc
来源：http://hz.hysaishi.cn/gtphmispaf.html

[R29] 定义函数
来源：http://hz.yueranfly.top/gtbztyepat.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.9152youxi.cn/gtntlymamn.html

[R30] 函数返回状态码
来源：http://hz.ywan-chungtsiang.top/gtuuvgbjsp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinghuilouyu.cn/gtwrorhqoq.html

[R31] 局部变量
来源：http://hz.aibaodan.cn/gtusxjgxpu.html

f() { local x=1; echo "$x"; }
来源：http://hz.c1oappe.top/gtjjreiyrl.html

[R32] 参数个数校验
来源：http://hz.jianghu66.top/gtfxgwckff.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gzhubu.top/gtqtiwrmiq.html

[R33] 捕获错误并提示行号
来源：http://hz.cqqwz.cn/gtpshmodwz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhoulong.xyz/gtgtmdcfqb.html

[R34] 退出时清理
来源：http://hz.9152youxi.cn/gtmusqmltw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtiaegajwb.html

[R35] 后台执行并等待
来源：http://hz.gogol.net.cn/gtxzzhxowc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.kuanghao11.cn/gtxnhyxick.html

[R36] 并发执行多个任务
来源：http://hz.shanyushiyangtech.top/gtkvfqsllm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj202588.top/gtxpedpumu.html

[R37] 把输出赋给变量
来源：http://hz.ivvv.top/gtctzwbvsw.html

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtugwglnvr.html

[R38] 管道串联
来源：http://hz.kuanghao11.cn/gtlfvxnazf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgufenzy.top/gtsicnqlke.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtskbfoalr.html

cmd > out.log 2>&1
来源：http://hz.zhijiandao.cn/gtvehzmprf.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtqcvsiddv.html

echo "log" >> out.log
来源：http://hz.sufxvd.cn/gtrftgkeix.html

[R41] 丢弃输出
来源：http://hz.jiagoushi.top/gttycwuqsa.html

cmd >/dev/null 2>&1
来源：http://hz.cqqwz.cn/gtyhpsnpmf.html

[R42] 输入重定向
来源：http://hz.ywan-chungtsiang.top/gtpudnqtbf.html

wc -l < a.txt
来源：http://hz.hysaishi.cn/gtwdkhvbiq.html

[R43] 按名字查找文件
来源：http://hz.ivvv.top/gtwcdvbgky.html

find . -name "*.log" -type f
来源：http://hz.aibaodan.cn/gtlchyuxjj.html

[R44] 按修改时间查找
来源：http://hz.zhixingplan.top/gtvmcmuhuz.html

find . -mtime -7 -type f
来源：http://hz.hywenlv.cn/gtswlswneg.html

[R45] 批量删除
来源：http://hz.meibo888.top/gtwjlyxeoc.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gtjvkreslk.html

[R46] 递归替换文件内容
来源：http://hz.yj20258888.top/gtfdlpnfaj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxinkj.top/gtvwufqlkt.html

[R47] sed 单行替换
来源：http://hz.aibaodan.cn/gtcwhsuynv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sysykeji.top/gtnhbcmqbx.html

[R48] awk 取指定列
来源：http://hz.chenjidiqi.icu/gtatrycgba.html

awk '{print $1, $3}' a.txt
来源：http://hz.ydzc1.top/gtkpmdgsvh.html

[R49] awk 带条件
来源：http://hz.havefunace.top/gtwilkayrd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.vqdsnc.cn/gtydnanzqu.html

[R50] awk 求和
来源：http://hz.tanke756.top/gttwidczpd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258.top/gttaeqftvh.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtzagalrsm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ybcxt.top/gtmyehpwbh.html

[R52] 统计行数
来源：http://hz.zhiwuduotai.top/gtlqwbnwpl.html

wc -l a.txt
来源：http://hz.jiagoushi.top/gtgwybhlrt.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgufenzy.top/gtwmgvhill.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtunuzgqpw.html

[R54] 比较两个文件
来源：http://hz.iojbl.cn/gtedhatuzy.html

diff a.txt b.txt
来源：http://hz.yanxiufei.cn/gtzluxlkxd.html

[R55] 压缩与解压
来源：http://hz.chenjidiqi.icu/gtqiapuocd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.andypj.xyz/gtqgiqijhh.html

[R56] 远程拷贝
来源：http://hz.shangyingyoupin.top/gtivjhohsd.html

scp file user@host:/path/
来源：http://hz.yanxiufei.cn/gtkqkidaqa.html

[R57] 远程执行命令
来源：http://hz.aibaodan.cn/gtjkgnrrcl.html

ssh user@host 'uptime'
来源：http://hz.zycfv.cn/gtozrvjqag.html

[R58] 下载文件
来源：http://hz.zdqjudy.top/gtnozrfjre.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.svipenyu.cn/gtulsgcggd.html

[R59] 发 POST JSON
来源：http://hz.svipenyu.cn/gtofufrlhp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhongyouzk.top/gtgzuilyhv.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gttugxyjtr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.bjfxy.top/gtcrkspehs.html

[R61] 磁盘占用
来源：http://hz.aizwys.cn/gtypirlpbd.html

df -h;  du -sh *
来源：http://hz.yongpay.top/gtpuikvnbv.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtvnklwemi.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258.top/gtazbgdqih.html

[R63] 内存与进程
来源：http://hz.hnqzz.top/gtncysgehp.html

free -h;  ps aux | grep nginx
来源：http://hz.sweek.top/gtdbkbshxs.html

[R64] 结束进程
来源：http://hz.jinghuilouyu.cn/gtbfgcnwlg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.wangshuangyany.cn/gtbpxmrkvi.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gttdwgdgyh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgfzy.top/gtabtvnsky.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtxalstsnm.html

crontab -e;  crontab -l
来源：http://hz.jqgufenzy.top/gtbibsnlre.html

[R67] 生成随机十六进制串
来源：http://hz.jyoumei.cn/gtdmylkhob.html

openssl rand -hex 16
来源：http://hz.sweek.top/gtixnqyziv.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtxeegoluq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtreqompqd.html

[R69] 生成随机密码
来源：http://hz.snrcjt.cn/gttcikkkas.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtlsploqqx.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtttcehwem.html

date +%s;  date -d @1700000000
来源：http://hz.dashuyun.cn/gtndvmcvzb.html

[R71] 日期格式化
来源：http://hz.hnqzz.top/gttwomcdtk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtrbfglvba.html

[R72] 等待端口就绪
来源：http://hz.jiagoushi.top/gtetcnepma.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aizwys.cn/gtgtnobezc.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gtqlmszfdl.html

split -l 1000 big.log part_
来源：http://hz.zhongyouzk.top/gtaqsumnms.html

[R74] 批量重命名
来源：http://hz.zhengqikj.top/gtllipvqyp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ivvv.top/gtoqfprkwt.html

[R75] 导出环境变量
来源：http://hz.xingfuxueyuan.xyz/gtblfmeorp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yonumen.top/gtyztbzetl.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtkieoxetb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtkzlphzdh.html

[R77] 读取用户输入
来源：http://hz.daria6918.cn/gtbtcdvnms.html

read -rp "请输入: " ans
来源：http://hz.9152youxi.cn/gtecmtjavn.html

[R78] 交互式菜单
来源：http://hz.sysykeji.top/gtnvymfsfb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.svipenyu.cn/gtsmpidyzi.html

[R79] 解析命令行选项
来源：http://hz.aizwys.cn/gtfgzifvxp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtmgglugui.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigufen.top/gtxlsjdcfn.html

time ./run.sh
来源：http://hz.zhijiandao.cn/gtsfpqtbft.html

================================================================================
来源：http://hz.chenzaomai.com/gtwnkogong.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gtgslinygr.html

================================================================================
来源：http://hz.pycfn.com/gtazibwjhx.html

[S01] C：Hello World
来源：http://hz.shzxlz.cn/gtpbimlkup.html

#include <stdio.h>
来源：http://hz.yuanzhike.top/gtsbkqtvqc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtdqbnkare.html

[S02] C：变量与格式化输出
来源：http://hz.ppjwa.cn/gtqvskeasm.html

int a = 10; printf("%d\n", a);
来源：http://hz.haohaochexian.top/gtjatyvtem.html

[S03] C：读入整数
来源：http://hz.dianchejie.cn/gtxcskicfk.html

int x; scanf("%d", &x);
来源：http://hz.yvedp.cn/gtcrwzvlnm.html

[S04] C：字符串复制
来源：http://hz.jinghuilouyu.cn/gtuscczcxz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gtfmnywqod.html

[S05] C：字符串长度
来源：http://hz.daxiang520.top/gtfiwxsgkd.html

strlen(s)
来源：http://hz.guannengcc.top/gtixutsmni.html

[S06] C：字符串比较
来源：http://hz.shanyushiyangtech.top/gtphbzjfsh.html

strcmp(a, b) == 0
来源：http://hz.nanxinkj.top/gtszdsnlbh.html

[S07] C：数组遍历求和
来源：http://hz.iojbl.cn/gtrulcdjjj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtgjttkagi.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gtufvqyedi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.feifeiyinyue.top/gtpjckrcuc.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gtjjczaufe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yvedp.cn/gtlwfkipmn.html

[S10] C：指针与解引用
来源：http://hz.cucudq.cn/gttalsswfp.html

int *p = &a;  *p = 5;
来源：http://hz.havefunace.top/gtocaauviw.html

[S11] C：逐行读文件
来源：http://hz.cqqwz.cn/gtzgruckvf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuetiantiany.cn/gtnubwxgmw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.c1oappe.top/gtssiwajzd.html

fclose(f);
来源：http://hz.jqgfzy.top/gtgooylyna.html

[S12] C：写文件
来源：http://hz.dianchejie.cn/gtwmscehzo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zdqjudy.top/gtpibbvtqp.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gttagonnmm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gtkytswqqm.html

[S14] C：枚举
来源：http://hz.sxryk.cn/gtzewdrfeg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtpngmumvg.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtfywnsfcm.html

(double) a / b
来源：http://hz.cheryme.top/gtfsuhvuwu.html

[S16] C：位操作置位
来源：http://hz.cucudq.cn/gtotkiizcd.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gtikufikwp.html

[S17] C：安全拼接字符串
来源：http://hz.hysaishi.cn/gtjnlmzqme.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj202588.top/gtsljyfbzj.html

[S18] C：命令行参数
来源：http://hz.cucudq.cn/gtilckdsmu.html

int main(int argc, char **argv)
来源：http://hz.hysaishi.cn/gtkijbkgfx.html

[S19] C：快速排序
来源：http://hz.redwolf501.top/gtpwhncqka.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gtqresnbak.html

[S20] C：二分查找
来源：http://hz.xziqi.cn/gttadcgyvq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtgpmcrliw.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtohfoyzyd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhaomingkeji.xyz/gtrjedbift.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gtlscgoxth.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.meibo888.top/gtnnqwxomi.html

[S23] C：随机数
来源：http://hz.hammf.cn/gtvcbmhypf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ppjwa.cn/gtyefhszaw.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtmvspqxmr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ybcxt.top/gtsbzdiwxo.html

[S25] C：内存拷贝
来源：http://hz.meibo888.top/gtbafgnleu.html

memcpy(dst, src, n);
来源：http://hz.quarkkingdee.top/gtylnmrqgo.html

[S26] C：内存清零
来源：http://hz.tianlin.xyz/gtrsbllsxq.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangkeji.top/gthlqjjhlz.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gtbazvmyiu.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtlczjmwso.html

[S28] C：静态变量
来源：http://hz.jinyuanbaomall.cn/gtimstujej.html

static int counter = 0;
来源：http://hz.sxryk.cn/gtaemepbei.html

[S29] C：变参函数
来源：http://hz.yueranfly.top/gtegasousw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxuanxn.top/gtdndlvkdr.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtgcycqzsa.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtyydbkrsy.html

#define X_H
来源：http://hz.daxiang520.top/gtumsupieh.html

#endif
来源：http://hz.zhoulong.xyz/gtsopomfco.html

[S31] C++：Hello World
来源：http://hz.yongpay.top/gtaumdwwpn.html

#include <iostream>
来源：http://hz.jiagoushi.top/gtqucagkkq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gthskacseq.html

[S32] C++：字符串
来源：http://hz.hongshengwenyu.top/gthtjnyuuo.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtghghsczc.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtinulrezf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhongyouzk.top/gtuvbwrfly.html

[S34] C++：遍历 vector
来源：http://hz.guannengcc.top/gtgrgsoayj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gtojkbwxit.html

[S35] C++：map
来源：http://hz.316326.xyz/gtbqelioao.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gthnuvxfja.html

[S36] C++：unordered_map
来源：http://hz.ybcxt.top/gtnctvyene.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gtwimzumox.html

[S37] C++：set
来源：http://hz.zdqjudy.top/gtrdpykgrc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xylfe.cn/gtxgcodzya.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtfejzuatd.html

std::sort(v.begin(), v.end());
来源：http://hz.mhx1999.top/gtshuigfiu.html

[S39] C++：自定义比较器排序
来源：http://hz.tanke756.top/gtncpkdtnr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gzhubu.top/gtvwfpaoey.html

[S40] C++：查找元素
来源：http://hz.cheryme.top/gtxunecswq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gthubesntc.html

[S41] C++：类与构造函数
来源：http://hz.yj20258888.top/gtskszcdnz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gtyktcknnt.html

[S42] C++：继承与虚函数
来源：http://hz.yanxiufei.cn/gtattmctjm.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhongyouzk.top/gtwxozqhed.html

[S43] C++：智能指针
来源：http://hz.gaohongyu789.top/gtywpdpbdq.html

auto p = std::make_unique<int>(5);
来源：http://hz.tian-w.cn/gtgzpzygwf.html

[S44] C++：引用传参
来源：http://hz.guowangkeji.top/gttvgimajp.html

void inc(int &x) { ++x; }
来源：http://hz.wangshuangyany.cn/gtoyibfpxq.html

[S45] C++：lambda
来源：http://hz.shanyushiyangtech.top/gtbpmgyybz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtuiegqdoa.html

[S46] C++：函数模板
来源：http://hz.pengpengdd.cyou/gtykjsgkts.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxuanxn.top/gtbqikadgx.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtbuzcrwhy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinyuanbaomall.cn/gtzgnzuvrg.html

[S48] C++：逐行读文件
来源：http://hz.316326.xyz/gtgxkjvggi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.guowangkeji.top/gtdtsdkjda.html

while (std::getline(in, line)) { }
来源：http://hz.sxryk.cn/gtxugrrzmz.html

[S49] C++：写文件
来源：http://hz.cqqwz.cn/gtbyugyugi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gttxmoevtq.html

[S50] C++：格式化数字
来源：http://hz.snrcjt.cn/gtqapcnfep.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj202588.top/gthzhpeddy.html

[S51] C++：显式类型转换
来源：http://hz.ehwqpu.com/gttsmramuu.html

static_cast<double>(a) / b
来源：http://hz.xuetiantiany.cn/gtrvzambvv.html

[S52] C++：const 与 noexcept
来源：http://hz.zhengqikj.top/gtasgmrvyu.html

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gthpffckla.html

[S53] C++：移动语义
来源：http://hz.sweek.top/gtgtnuiuer.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtbqjjosvc.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtebzvpwfe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daxiang520.top/gtsrdzdxhq.html

[S55] C++：结构化绑定
来源：http://hz.52xcode.cn/gtgnuhmlag.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gtgplpaxhl.html

[S56] C++：optional
来源：http://hz.nanxuanxn.top/gtxzhavnhr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinghuilouyu.cn/gtfmajzscs.html

[S57] C++：编译期常量
来源：http://hz.yuxming.cn/gtyjoinjjg.html

constexpr int N = 10;
来源：http://hz.iojbl.cn/gthggavmfm.html

[S58] C++：命名空间
来源：http://hz.andypj.xyz/gttkabhbrx.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangkeji.top/gtqwjjikjq.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gtamzwkfvn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daria6918.cn/gtbnnoflfp.html

[S60] C++：遍历并删除元素
来源：http://hz.iojbl.cn/gtipfazehw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aizwys.cn/gtqckuuspi.html

================================================================================
来源：http://hz.ydzc1.top/gtiqrnymut.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.feifeiyinyue.top/gtslpdbblj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjzmwqoys.html


<!-- 参考信息 -->