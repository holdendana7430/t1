代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.ydzc1.top/gtaccpweyc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.snrcjt.cn/gtkhchobch.html

[Q83] 大小写转换
来源：http://hz.fengsongda.top/gtjtlzquun.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtlbspecxk.html

[Q84] 去除首尾空格
来源：http://hz.mhx1999.top/gtkptgcpze.html

SELECT TRIM(name) FROM users;
来源：http://hz.yvedp.cn/gtrbczteqf.html

[Q85] 数值取整
来源：http://hz.xingfuxueyuan.xyz/gtxffhirtv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yanxiufei.cn/gtyifkpyhp.html

[Q86] 读取 JSON 字段
来源：http://hz.quarkkingdee.top/gtewfydabe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hfpthk.cn/gtkxkcxwgs.html

[Q87] JSON 字段做条件
来源：http://hz.316326.xyz/gtjahwdkaw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tanke756.top/gtzxxowood.html

[Q88] 行转列（条件聚合）
来源：http://hz.havefunace.top/gtbeqqbttw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hammf.cn/gtqdtivalt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shuidangran.top/gtnrdptoiw.html

[Q89] 判断表是否存在
来源：http://hz.ydzc1.top/gtskapqicc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guannengcc.top/gtusxvnkyi.html

[Q90] 生成序号列
来源：http://hz.zhaomingkeji.xyz/gtkwulvbur.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtbekzlruq.html

================================================================================
来源：http://hz.cheryme.top/gtrjzxedle.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gtdmyauzhw.html

================================================================================
来源：http://hz.meibo888.top/gtehorsnim.html

[R01] shebang 与严格模式
来源：http://hz.hfpthk.cn/gtcavjvbxi.html

#!/usr/bin/env bash
来源：http://hz.fzhhl.top/gtozgrdxrf.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtyvluxjqv.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gttltztuzm.html

name="Tom"; echo "$name"
来源：http://hz.ydzc1.top/gtpkfnomuk.html

[R03] 只读变量
来源：http://hz.jinghuilouyu.cn/gtrscjgamg.html

readonly PI=3.14
来源：http://hz.ivvv.top/gtsgtjgofo.html

[R04] 位置参数
来源：http://hz.jinqigufen.top/gtiwdkwdhc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ivvv.top/gtvkyjuegc.html

[R05] 参数默认值
来源：http://hz.sysykeji.top/gthqjyxjdf.html

name="${1:-default}"
来源：http://hz.andypj.xyz/gtwmrdecwu.html

[R06] 判断命令是否存在
来源：http://hz.zhongyouzk.top/gtzpaufemz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgfzy.top/gtbjreacsd.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtwosufpux.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shuidangran.top/gttxftlhzz.html

[R08] 数值比较
来源：http://hz.meibo888.top/gtbgemcydg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.0kj1m.cn/gtcapwkche.html

[R09] 字符串比较
来源：http://hz.quarkkingdee.top/gtcdibvsoe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xziqi.cn/gthmsjhgyg.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtxtdpsyfe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.wangdashe.top/gtblhbjymo.html

[R11] case 多分支
来源：http://hz.iojbl.cn/gtpmfuzbra.html

case "$1" in
来源：http://hz.jinghuilouyu.cn/gtlddplzpa.html

start) echo "启动" ;;
来源：http://hz.tianlin.xyz/gtmhpnxrop.html

stop)  echo "停止" ;;
来源：http://hz.gzhubu.top/gtekslswhu.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gtrftvsrlp.html

esac
来源：http://hz.xylfe.cn/gtiqotxput.html

[R12] for 遍历文件
来源：http://hz.ydzc1.top/gtzbuizxyb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtqglqpdpd.html

[R13] for 计数循环
来源：http://hz.shuidangran.top/gtfmdaokbb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.svipenyu.cn/gtqxnsegbi.html

[R14] C 风格 for
来源：http://hz.cucudq.cn/gtrlczkbgb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.redwolf501.top/gtjakrhshd.html

[R15] while 逐行读文件
来源：http://hz.tianlin.xyz/gtucfemnxm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gthzxbswhz.html

[R16] until 等待条件
来源：http://hz.zhixingplan.top/gtikrtuqef.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dashuyun.cn/gtrfiwnloa.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtflnlygkx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258.top/gtpxarlvsw.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gtcmktstos.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yueranfly.top/gtxvpjzxol.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtpdlusblk.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtnrbugnmb.html

[R20] 关联数组（字典）
来源：http://hz.dianchejie.cn/gtyknfcxyb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hnqzz.top/gtzzppfaxz.html

[R21] 字符串长度
来源：http://hz.sweek.top/gtxxdntsea.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtpplpwptr.html

[R22] 截取子串
来源：http://hz.aibaodan.cn/gtopzlqmde.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtlagbtauq.html

[R23] 字符串替换
来源：http://hz.wangshuangyany.cn/gtyaucaloz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.9152youxi.cn/gtuxafraiy.html

[R24] 大小写转换
来源：http://hz.hnqzz.top/gteuxtcrou.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gtbkysqlyb.html

[R25] 去后缀 / 去前缀
来源：http://hz.aizwys.cn/gtglwhfhzg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fengsongda.top/gtuvffiufl.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtczjtmjgp.html

now=$(date +%F); echo "$now"
来源：http://hz.yongpay.top/gtfdozhrmc.html

[R27] 算术展开
来源：http://hz.birdmap.top/gtfboxclva.html

echo $((1 + 2 * 3))
来源：http://hz.ybcxt.top/gtilvwlbbz.html

[R28] 浮点运算
来源：http://hz.nanxinkj.top/gttlawzwdq.html

echo "scale=2; 10/3" | bc
来源：http://hz.bjfxy.top/gtufeqozvx.html

[R29] 定义函数
来源：http://hz.nanxinkj.top/gtmsadasxn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gaohongyu789.top/gtssvuzibl.html

[R30] 函数返回状态码
来源：http://hz.xingfuxueyuan.xyz/gtsfmqgqmd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sysykeji.top/gtobcgybpo.html

[R31] 局部变量
来源：http://hz.kuanghao11.cn/gtudjlxwzj.html

f() { local x=1; echo "$x"; }
来源：http://hz.0kj1m.cn/gtcwmozjuk.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gthqgxglml.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtvoxuwbif.html

[R33] 捕获错误并提示行号
来源：http://hz.sweek.top/gtmqwmcxzf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gtefqhoktz.html

[R34] 退出时清理
来源：http://hz.yongpay.top/gtzvxgwdbd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtvgcgjxuz.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtfsjzodws.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yanxiufei.cn/gtzrbxgcky.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gtmytbvqep.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.haohaochexian.top/gtmhhvgvwc.html

[R37] 把输出赋给变量
来源：http://hz.nanxuanxn.top/gthiryaabn.html

files=$(ls -1)
来源：http://hz.snrcjt.cn/gtcyhydisd.html

[R38] 管道串联
来源：http://hz.yongpay.top/gtouliaihs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.52xcode.cn/gtnaoezbow.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gtddzragat.html

cmd > out.log 2>&1
来源：http://hz.jyoumei.cn/gtsjqujgrv.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtnlzxlden.html

echo "log" >> out.log
来源：http://hz.fzhhl.top/gtpcrzhyqe.html

[R41] 丢弃输出
来源：http://hz.xingfuxueyuan.xyz/gtudfhmcwv.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258888.top/gtqlgctdep.html

[R42] 输入重定向
来源：http://hz.kuanghao11.cn/gttybegxcz.html

wc -l < a.txt
来源：http://hz.chenzaomai.com/gtqlybswan.html

[R43] 按名字查找文件
来源：http://hz.aizwys.cn/gtqkzqtqte.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gtgyhwhqln.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtidjhyxis.html

find . -mtime -7 -type f
来源：http://hz.gaohongyu789.top/gtsnyxkbig.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtnubsbuqi.html

find . -name "*.tmp" -delete
来源：http://hz.yuanzhike.top/gtsvgduuxn.html

[R46] 递归替换文件内容
来源：http://hz.jyoumei.cn/gtclsovkqi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangshuangyany.cn/gtzpkajoco.html

[R47] sed 单行替换
来源：http://hz.feifeiyinyue.top/gtfprvxzlq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yangfankeji.com/gtbchrksla.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gtkxyayjaj.html

awk '{print $1, $3}' a.txt
来源：http://hz.gogol.net.cn/gtygojgcur.html

[R49] awk 带条件
来源：http://hz.hammf.cn/gtqzjraduo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gogol.net.cn/gtvtzgjnsu.html

[R50] awk 求和
来源：http://hz.hfpthk.cn/gtsnyyclnl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xylfe.cn/gtjpkiveqy.html

[R51] 排序去重取前几
来源：http://hz.ywan-chungtsiang.top/gtllqdujyx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtokurtcfm.html

[R52] 统计行数
来源：http://hz.hongshengwenyu.top/gtcejnmhru.html

wc -l a.txt
来源：http://hz.redwolf501.top/gtbaadsezy.html

[R53] 查看文件头与实时尾
来源：http://hz.jinyuanbaomall.cn/gtoievpzdq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj202588.top/gtxvsvnobp.html

[R54] 比较两个文件
来源：http://hz.yanxiufei.cn/gtpvxucxbs.html

diff a.txt b.txt
来源：http://hz.feifeiyinyue.top/gtfdkcnags.html

[R55] 压缩与解压
来源：http://hz.zdqjudy.top/gthrpstfkx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgufenzy.top/gtxchhfrdy.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtgpbggoxb.html

scp file user@host:/path/
来源：http://hz.jinqigfzy.top/gtdecontzb.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtvwiqpjjr.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtgxesgpde.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtuuzjcddw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.0kj1m.cn/gtsuvvpmxz.html

[R59] 发 POST JSON
来源：http://hz.daria6918.cn/gtvkumyvan.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fengsongda.top/gtfklkprfd.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtfxtnsiiv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtsariqthu.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gtrywmqnyb.html

df -h;  du -sh *
来源：http://hz.ybcxt.top/gtkfrtzkks.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gtodmzlubr.html

du -ah . | sort -rh | head -10
来源：http://hz.sxryk.cn/gtyimksgem.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtfxhkvcbg.html

free -h;  ps aux | grep nginx
来源：http://hz.smart0.xyz/gtashdzfah.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtbqrdyulk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.svipenyu.cn/gtxtfbgdyb.html

[R65] 查看端口占用
来源：http://hz.jinyuanbaomall.cn/gtpanwxbmn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigufen.top/gtojqjkmgm.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtaqreespd.html

crontab -e;  crontab -l
来源：http://hz.c1oappe.top/gtxlwzmrtn.html

[R67] 生成随机十六进制串
来源：http://hz.bjfxy.top/gtluhlorof.html

openssl rand -hex 16
来源：http://hz.vqdsnc.cn/gtvjdjsdlo.html

[R68] 计算文件校验值
来源：http://hz.52xcode.cn/gtapehqmfs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yangfankeji.com/gtloyofoxj.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gthqmtlbra.html

head -c 16 /dev/urandom | base64
来源：http://hz.wangdashe.top/gtrqcqcuht.html

[R70] 时间戳与互转
来源：http://hz.yangfankeji.com/gtfjxsnhpg.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtissnqqqa.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtpnuthttz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.quarkkingdee.top/gtqooyugeq.html

[R72] 等待端口就绪
来源：http://hz.aibaodan.cn/gtlevroazy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xuetiantiany.cn/gtrreljqqd.html

[R73] 分割大日志
来源：http://hz.pycfn.com/gtjkwmpphu.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gthdchldla.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtvddayyce.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtfcjjfver.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangtech.top/gtnccxetom.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtlmenqorw.html

[R76] 使用临时文件
来源：http://hz.jinqigfzy.top/gtquypaiga.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtunzwzlka.html

[R77] 读取用户输入
来源：http://hz.jinyuanbaomall.cn/gtfbmocrsl.html

read -rp "请输入: " ans
来源：http://hz.jqgufenzy.top/gtssmcloht.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtuptggodj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ppjwa.cn/gtlyesyrkw.html

[R79] 解析命令行选项
来源：http://hz.zhiwuduotai.top/gtiplduqek.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtwqjdiosv.html

[R80] 查看脚本执行耗时
来源：http://hz.hammf.cn/gtyrbebwvh.html

time ./run.sh
来源：http://hz.nwbrower.top/gtqigdhqgq.html

================================================================================
来源：http://hz.52xcode.cn/gtozydwnrh.html

S. C / C++ 专题
来源：http://hz.daxiang520.top/gthdryfnkb.html

================================================================================
来源：http://hz.dianchejie.cn/gtjncxofgi.html

[S01] C：Hello World
来源：http://hz.hammf.cn/gtbpmbjnzo.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtaqhsstvs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shangyingyoupin.top/gtdmsbdhjn.html

[S02] C：变量与格式化输出
来源：http://hz.yuanzhike.top/gtqtpeydbd.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gthsskpolj.html

[S03] C：读入整数
来源：http://hz.gogol.net.cn/gtfmvasceh.html

int x; scanf("%d", &x);
来源：http://hz.aibaodan.cn/gtrthrmmqn.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtuwsvysgx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhixingplan.top/gtufvnbdrl.html

[S05] C：字符串长度
来源：http://hz.daria6918.cn/gtosziulrw.html

strlen(s)
来源：http://hz.cdnleiting.top/gtghzmqcep.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtnnipiknc.html

strcmp(a, b) == 0
来源：http://hz.ivvv.top/gtiipjdkmf.html

[S07] C：数组遍历求和
来源：http://hz.iojbl.cn/gtfjdalczj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hysaishi.cn/gtixszwblo.html

[S08] C：动态内存分配与释放
来源：http://hz.jlsjyb.cn/gtfsdjqxkp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xinyue.icu/gtadyqenmx.html

[S09] C：结构体定义与初始化
来源：http://hz.aizwys.cn/gtlzwhemyl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuanzx.com/gtugpaajad.html

[S10] C：指针与解引用
来源：http://hz.jqgfzy.top/gtjtqxrhiy.html

int *p = &a;  *p = 5;
来源：http://hz.sweek.top/gttrwtqwyz.html

[S11] C：逐行读文件
来源：http://hz.9152youxi.cn/gtihcdjlfi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.birdmap.top/gtfhpmxxpo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.kuanghao11.cn/gtwnbcpnpx.html

fclose(f);
来源：http://hz.snrcjt.cn/gtssvckrgb.html

[S12] C：写文件
来源：http://hz.yuanzhike.top/gtpfgduycc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jyoumei.cn/gtddapmlcu.html

[S13] C：宏定义
来源：http://hz.xuanzx.com/gtoncoxjmx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jyoumei.cn/gtgymmhivi.html

[S14] C：枚举
来源：http://hz.mhx1999.top/gtodgplpyp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.c1oappe.top/gtaobbtnnj.html

[S15] C：类型转换
来源：http://hz.zhiwuduotai.top/gtzqruybdd.html

(double) a / b
来源：http://hz.pengpengdd.cyou/gtaryfzugi.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gtpqvsbwgq.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtqqjgubkd.html

[S17] C：安全拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtjoenozqq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tian-w.cn/gtauhopubw.html

[S18] C：命令行参数
来源：http://hz.c1oappe.top/gtzsdwnvtu.html

int main(int argc, char **argv)
来源：http://hz.jiagoushi.top/gtxsgrbphg.html

[S19] C：快速排序
来源：http://hz.gogol.net.cn/gtryyamfdl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtsiacbauw.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gttbswvaxf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtglrqpara.html

[S21] C：字符类别判断
来源：http://hz.gotoacloud.top/gtnuvsqhnq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj202588.top/gtdqqqmzlo.html

[S22] C：字符串转数字
来源：http://hz.xuanzx.com/gtochxlgup.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shzxlz.cn/gtctlgscns.html

[S23] C：随机数
来源：http://hz.guowangkeji.top/gtvexsmdbb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gogol.net.cn/gtlxrjnxoo.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gtuhknbmyf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tianlin.xyz/gtdabtnzrp.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtekmbqvkp.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtothnlkyc.html

[S26] C：内存清零
来源：http://hz.havefunace.top/gtpaaxwidp.html

memset(a, 0, sizeof a);
来源：http://hz.andypj.xyz/gtryvyusmq.html

[S27] C：定义常量
来源：http://hz.9152youxi.cn/gtgwxavlci.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtfpgrijzo.html

[S28] C：静态变量
来源：http://hz.c1oappe.top/gtelvjmues.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtmeqddlas.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gtklrrcvwq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cucudq.cn/gtrsumleba.html

[S30] C：头文件保护
来源：http://hz.xziqi.cn/gtpeienzde.html

#ifndef X_H
来源：http://hz.jinghuilouyu.cn/gtfohacuzc.html

#define X_H
来源：http://hz.zhaomingkeji.xyz/gtpbefjkke.html

#endif
来源：http://hz.xinyue.icu/gtwizistre.html

[S31] C++：Hello World
来源：http://hz.vqdsnc.cn/gtgqvlispk.html

#include <iostream>
来源：http://hz.aizwys.cn/gtzcrcvlgm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gogol.net.cn/gtuhabusyh.html

[S32] C++：字符串
来源：http://hz.gzhubu.top/gtklopnygy.html

std::string s = "hi";  s += "!";
来源：http://hz.fengsongda.top/gtuuvjeqxp.html

[S33] C++：vector 增删
来源：http://hz.yj202588.top/gtskkmvrxy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ppjwa.cn/gtfvmhtosj.html

[S34] C++：遍历 vector
来源：http://hz.sxryk.cn/gtgfduxtfc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jyoumei.cn/gtgddfuawo.html

[S35] C++：map
来源：http://hz.gzhubu.top/gtkjdpmrto.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtegdwblre.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gtomatkjzn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtyjyztmcp.html

[S37] C++：set
来源：http://hz.hongshengwenyu.top/gtxgxeedhu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangtech.top/gtfqrfrxwl.html

[S38] C++：排序
来源：http://hz.zhongyouzk.top/gtwgzyitll.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtykphqdwg.html

[S39] C++：自定义比较器排序
来源：http://hz.dashuyun.cn/gtlhmujltx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.haohaochexian.top/gtewnzskjz.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtjikjqado.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinghuilouyu.cn/gtoldljqdm.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtcxhyjivl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhengqikj.top/gttqzazxki.html

[S42] C++：继承与虚函数
来源：http://hz.yuxming.cn/gtkhvmwkin.html

class B : public Base { public: void f() override {} };
来源：http://hz.52xcode.cn/gtwmljkhzh.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtlyvmnijc.html

auto p = std::make_unique<int>(5);
来源：http://hz.yvedp.cn/gtfaqnbuuz.html

[S44] C++：引用传参
来源：http://hz.yuxming.cn/gtuegcjocq.html

void inc(int &x) { ++x; }
来源：http://hz.dashuyun.cn/gtkashtqbt.html

[S45] C++：lambda
来源：http://hz.xinyue.icu/gtmovwzyjv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guannengcc.top/gtfkrmxfdx.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtjcahkurb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangdashe.top/gtajzdztxf.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gttrfwehvp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtlnxneifk.html

[S48] C++：逐行读文件
来源：http://hz.yuxming.cn/gtzeggnjqc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jyoumei.cn/gtcfqwooiw.html

while (std::getline(in, line)) { }
来源：http://hz.chenlongwang.top/gtfotjvbym.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtxhgonwvj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtdcddovxz.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtjycsduaw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guowangkeji.top/gtauwcldoz.html

[S51] C++：显式类型转换
来源：http://hz.xylfe.cn/gtxtddijgn.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtjweeopwq.html

[S52] C++：const 与 noexcept
来源：http://hz.fengsongda.top/gtdmfpxetk.html


<!-- 参考信息 -->