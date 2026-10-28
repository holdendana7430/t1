代发 wailian999

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtngesfnui.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gteycudgep.html

[Q87] JSON 字段做条件
来源：http://hz.meibo888.top/gtuhczmcmd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.meibo888.top/gtbramfczt.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenjidiqi.icu/gtejteezgl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtimyorggq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xinyue.icu/gtexvtaolk.html

[Q89] 判断表是否存在
来源：http://hz.xuanzx.com/gtbhggdskc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtwhzrknil.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtsbrrzcsl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gzhubu.top/gtclmyrjvp.html

================================================================================
来源：http://hz.gogol.net.cn/gtljtjaddo.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtvluqbybt.html

================================================================================
来源：http://hz.jqgufenzy.top/gtatbysspj.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gtgxencevq.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtdmbviden.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtlvwuxzkv.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gtqmtzkamf.html

name="Tom"; echo "$name"
来源：http://hz.c1oappe.top/gttypnuvdu.html

[R03] 只读变量
来源：http://hz.zycfv.cn/gtnxxfdqpc.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtfplciciz.html

[R04] 位置参数
来源：http://hz.jqgufenzy.top/gtslvncxui.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jyoumei.cn/gtbqamnujl.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gtdjqogcjm.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtrtylwgay.html

[R06] 判断命令是否存在
来源：http://hz.jyoumei.cn/gttkryalmt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtrrkqglnl.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtjedztqft.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sysykeji.top/gtvvlnbbpa.html

[R08] 数值比较
来源：http://hz.haohaochexian.top/gtrrrbbnnu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cqqwz.cn/gtnjbfvccm.html

[R09] 字符串比较
来源：http://hz.yj20258.top/gtetnvyunz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtolemfqug.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gthbukigph.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ybcxt.top/gtcwtfjhyk.html

[R11] case 多分支
来源：http://hz.xziqi.cn/gtlrabqjru.html

case "$1" in
来源：http://hz.gaohongyu789.top/gthzqkcbhn.html

start) echo "启动" ;;
来源：http://hz.jinqigufen.top/gtywdnjagw.html

stop)  echo "停止" ;;
来源：http://hz.zhoulong.xyz/gtejxdopph.html

*)     echo "未知命令" ;;
来源：http://hz.mhx1999.top/gtfgxxowqe.html

esac
来源：http://hz.snrcjt.cn/gtgveflwrn.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtorsmlzzh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gtiqresrlz.html

[R13] for 计数循环
来源：http://hz.sufxvd.cn/gtmtsvkzqc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gtdxmwfiog.html

[R14] C 风格 for
来源：http://hz.shzxlz.cn/gtvwnstcmd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtyttcvnmb.html

[R15] while 逐行读文件
来源：http://hz.fengsongda.top/gtsjwcywyh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sweek.top/gtitctwcbe.html

[R16] until 等待条件
来源：http://hz.dianchejie.cn/gtuxwlnals.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.52xcode.cn/gtkksrxytf.html

[R17] 数组定义与取值
来源：http://hz.andypj.xyz/gtfazvikdh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenlongwang.top/gthetagrgi.html

[R18] 遍历数组
来源：http://hz.hysaishi.cn/gtdvkatjpk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhijiandao.cn/gtksouhqej.html

[R19] 数组长度
来源：http://hz.guowangkeji.top/gtbjtpeahh.html

echo "${#arr[@]}"
来源：http://hz.cqqwz.cn/gtrdqmvgtl.html

[R20] 关联数组（字典）
来源：http://hz.xinyue.icu/gthncnfnnn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtxgxjgmie.html

[R21] 字符串长度
来源：http://hz.iojbl.cn/gtcxcgczkg.html

echo "${#s}"
来源：http://hz.yj202588.top/gtdjwladkr.html

[R22] 截取子串
来源：http://hz.pengpengdd.cyou/gttjkjuaky.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtgrtzlequ.html

[R23] 字符串替换
来源：http://hz.9152youxi.cn/gtoircyytf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ehwqpu.com/gtqroqgsiu.html

[R24] 大小写转换
来源：http://hz.hnqzz.top/gtjlwgnhor.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hongshengwenyu.top/gtxalewrcp.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuxming.cn/gtafbqzono.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zycfv.cn/gtmlljcmod.html

[R26] 命令替换
来源：http://hz.hywenlv.cn/gtbgihdhxi.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gtgfyokwql.html

[R27] 算术展开
来源：http://hz.iojbl.cn/gttecfhuvr.html

echo $((1 + 2 * 3))
来源：http://hz.cheryme.top/gtdlysftuk.html

[R28] 浮点运算
来源：http://hz.yvedp.cn/gtriehewhm.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gtednnpkqp.html

[R29] 定义函数
来源：http://hz.cucudq.cn/gtilkomucs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ehwqpu.com/gtulobiaja.html

[R30] 函数返回状态码
来源：http://hz.xuanzx.com/gtgrtvckad.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cucudq.cn/gtzrrqbhxb.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtepslqczv.html

f() { local x=1; echo "$x"; }
来源：http://hz.jlsjyb.cn/gthrgtvdbj.html

[R32] 参数个数校验
来源：http://hz.dianchejie.cn/gthzzcoqrn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtdbuhzsbx.html

[R33] 捕获错误并提示行号
来源：http://hz.jinqigfzy.top/gtivazvjzg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhoulong.xyz/gtttsnyjoa.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtlfxthfia.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gttqinbpjz.html

[R35] 后台执行并等待
来源：http://hz.ehwqpu.com/gtosoqaxtc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gthpdstrwh.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtwujpjkkb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gotoacloud.top/gtlvaosctv.html

[R37] 把输出赋给变量
来源：http://hz.sufxvd.cn/gtprasrrys.html

files=$(ls -1)
来源：http://hz.xingfuxueyuan.xyz/gtjxohtedy.html

[R38] 管道串联
来源：http://hz.gaohongyu789.top/gtxlwdbxjm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yueranfly.top/gtuwyqayks.html

[R39] 重定向标准输出与错误
来源：http://hz.hongshengwenyu.top/gtfmplnzbi.html

cmd > out.log 2>&1
来源：http://hz.smart0.xyz/gtyajhufgh.html

[R40] 追加写日志
来源：http://hz.yj20258.top/gtlsvkopuh.html

echo "log" >> out.log
来源：http://hz.tian-w.cn/gtzzueoqsa.html

[R41] 丢弃输出
来源：http://hz.cheryme.top/gtcqsvmjrp.html

cmd >/dev/null 2>&1
来源：http://hz.nanxuanxn.top/gtrxkqkyrj.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtjszktrsr.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtdxigjtrg.html

[R43] 按名字查找文件
来源：http://hz.ppjwa.cn/gtpuckdzic.html

find . -name "*.log" -type f
来源：http://hz.yanxiufei.cn/gtcbafqdll.html

[R44] 按修改时间查找
来源：http://hz.wangdashe.top/gtekexxosm.html

find . -mtime -7 -type f
来源：http://hz.daria6918.cn/gtoslnsmjh.html

[R45] 批量删除
来源：http://hz.dashuyun.cn/gtnxupytvf.html

find . -name "*.tmp" -delete
来源：http://hz.aibaodan.cn/gteuwbhruy.html

[R46] 递归替换文件内容
来源：http://hz.yangfankeji.com/gtuudzvijk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenzaomai.com/gtqemmkynx.html

[R47] sed 单行替换
来源：http://hz.cucudq.cn/gtzqruvrde.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nwbrower.top/gtaymodhyy.html

[R48] awk 取指定列
来源：http://hz.yj202588.top/gtfgxflldx.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgufenzy.top/gtilcwjoqc.html

[R49] awk 带条件
来源：http://hz.chenjidiqi.icu/gtpcmcdtbf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtjeylngcu.html

[R50] awk 求和
来源：http://hz.fengsongda.top/gtjvazikdr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258.top/gtbzklvyzu.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtfjztltfk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jlsjyb.cn/gtuxdugmhg.html

[R52] 统计行数
来源：http://hz.wangdashe.top/gthujxkdrv.html

wc -l a.txt
来源：http://hz.ydzc1.top/gtplhvbzfh.html

[R53] 查看文件头与实时尾
来源：http://hz.hongshengwenyu.top/gtmbdyfzgr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gtttlfxghu.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtogprgxow.html

diff a.txt b.txt
来源：http://hz.guannengcc.top/gtsgecyzlb.html

[R55] 压缩与解压
来源：http://hz.ehwqpu.com/gtostwuxwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuanzx.com/gtbeffaaow.html

[R56] 远程拷贝
来源：http://hz.316326.xyz/gtfftkygqm.html

scp file user@host:/path/
来源：http://hz.zhengqikj.top/gtibusctst.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gttrkohlma.html

ssh user@host 'uptime'
来源：http://hz.gotoacloud.top/gtduwgoepk.html

[R58] 下载文件
来源：http://hz.pycfn.com/gtcdbthioy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tian-w.cn/gtxgtpnpcy.html

[R59] 发 POST JSON
来源：http://hz.kuanghao11.cn/gtfrzkcxct.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hammf.cn/gtrlxkfefz.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtlphfvqsz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sxryk.cn/gtnctjlelr.html

[R61] 磁盘占用
来源：http://hz.andypj.xyz/gtrpdsnktz.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtjewbwuam.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtydvohffp.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangtech.top/gtpreytwrs.html

[R63] 内存与进程
来源：http://hz.ydjk.org.cn/gtfxlledqc.html

free -h;  ps aux | grep nginx
来源：http://hz.xziqi.cn/gtszknrpju.html

[R64] 结束进程
来源：http://hz.shuidangran.top/gtrkjphpmt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ppjwa.cn/gtvedromlh.html

[R65] 查看端口占用
来源：http://hz.zhengqikj.top/gtkrszgkxi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtsgbtswkk.html

[R66] 定时任务
来源：http://hz.zdqjudy.top/gtxgygpvpl.html

crontab -e;  crontab -l
来源：http://hz.dashuyun.cn/gtfwabpwqq.html

[R67] 生成随机十六进制串
来源：http://hz.cheryme.top/gtymudogpu.html

openssl rand -hex 16
来源：http://hz.hongshengwenyu.top/gtbvrrrjci.html

[R68] 计算文件校验值
来源：http://hz.daria6918.cn/gtlbrkxmtu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgufenzy.top/gttzpajora.html

[R69] 生成随机密码
来源：http://hz.xylfe.cn/gtllhgakkj.html

head -c 16 /dev/urandom | base64
来源：http://hz.cashguo.top/gtohofmcpo.html

[R70] 时间戳与互转
来源：http://hz.jianghu66.top/gtwwzbefax.html

date +%s;  date -d @1700000000
来源：http://hz.cdnleiting.top/gtchnuhuue.html

[R71] 日期格式化
来源：http://hz.ehwqpu.com/gtwkhgiywn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sweek.top/gtmeinmhmt.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtomgbnghz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yonumen.top/gtbotfkxll.html

[R73] 分割大日志
来源：http://hz.sweek.top/gtucwizpmh.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtabfpoytv.html

[R74] 批量重命名
来源：http://hz.chenlongwang.top/gtyfvaavhs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gtwlvfmuyy.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtinsqoegu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtrovauivb.html

[R76] 使用临时文件
来源：http://hz.hnqzz.top/gtvrxqzlud.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gtablqubaz.html

[R77] 读取用户输入
来源：http://hz.yvedp.cn/gtpxprjapa.html

read -rp "请输入: " ans
来源：http://hz.wangdashe.top/gtqujzwogt.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtlatmfsda.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgufenzy.top/gtqfvppejq.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gtpcsbtrce.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zycfv.cn/gtbarbmcgt.html

[R80] 查看脚本执行耗时
来源：http://hz.feifeiyinyue.top/gtuikjgveb.html

time ./run.sh
来源：http://hz.9152youxi.cn/gtrwsmyvln.html

================================================================================
来源：http://hz.hysaishi.cn/gtakevlqps.html

S. C / C++ 专题
来源：http://hz.pycfn.com/gtemkylnwt.html

================================================================================
来源：http://hz.smart0.xyz/gtaqylmdlx.html

[S01] C：Hello World
来源：http://hz.hongshengwenyu.top/gtqdadaiwb.html

#include <stdio.h>
来源：http://hz.hnqzz.top/gtlrxexxvw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydzc1.top/gtwjfrmabf.html

[S02] C：变量与格式化输出
来源：http://hz.yongpay.top/gtpbudqteh.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gtfdsqdvxd.html

[S03] C：读入整数
来源：http://hz.ydzc1.top/gtgypliuyj.html

int x; scanf("%d", &x);
来源：http://hz.aibaodan.cn/gtwjqgirte.html

[S04] C：字符串复制
来源：http://hz.jinyuanbaomall.cn/gttzbuwros.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtprgqrpuu.html

[S05] C：字符串长度
来源：http://hz.vqdsnc.cn/gtnsdysbet.html

strlen(s)
来源：http://hz.redwolf501.top/gtmahecvkj.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gthowcfkkn.html

strcmp(a, b) == 0
来源：http://hz.sxryk.cn/gtspykdmgx.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtbwwssjqx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtdmmtawhg.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtqxztnksz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gthlonelbr.html

[S09] C：结构体定义与初始化
来源：http://hz.redwolf501.top/gtczwevgzq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtoeeutthh.html

[S10] C：指针与解引用
来源：http://hz.nanxinkj.top/gtnmtmdhau.html

int *p = &a;  *p = 5;
来源：http://hz.sxryk.cn/gtpgizcvev.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtngyisgox.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxinkj.top/gtgfnzlbdl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jyoumei.cn/gtznagyijj.html

fclose(f);
来源：http://hz.tianlin.xyz/gteblhfsnn.html

[S12] C：写文件
来源：http://hz.redwolf501.top/gtfyhhbtgb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.redwolf501.top/gtbqkhddgr.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtdqjjxhis.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sysykeji.top/gthdpqqcei.html

[S14] C：枚举
来源：http://hz.jyoumei.cn/gtlhnsmooi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jlsjyb.cn/gtfyrpdlwp.html

[S15] C：类型转换
来源：http://hz.pengpengdd.cyou/gtxcehtfgl.html

(double) a / b
来源：http://hz.xziqi.cn/gtrszidgag.html

[S16] C：位操作置位
来源：http://hz.iojbl.cn/gtzebeneew.html

x |= (1 << 3);
来源：http://hz.sufxvd.cn/gtieujqeij.html

[S17] C：安全拼接字符串
来源：http://hz.ydjk.org.cn/gtuglrofgo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jiagoushi.top/gtlyrxgibg.html

[S18] C：命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtoyvxgfkb.html

int main(int argc, char **argv)
来源：http://hz.yongpay.top/gtlbcmtqzf.html

[S19] C：快速排序
来源：http://hz.c1oappe.top/gtnygczyyj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtququjpoy.html

[S20] C：二分查找
来源：http://hz.daria6918.cn/gtadihgkyr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gthnqzarry.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtgpxtxqtb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.mhx1999.top/gtphhoddpv.html

[S22] C：字符串转数字
来源：http://hz.gzhubu.top/gtjmiazqlx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fzhhl.top/gtenjfkgfl.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtvtwmumlw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinghuilouyu.cn/gtlfichrgf.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtiijguosb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.meibo888.top/gtolvufpgp.html

[S25] C：内存拷贝
来源：http://hz.yueranfly.top/gtqfmjuaah.html

memcpy(dst, src, n);
来源：http://hz.cheryme.top/gtcdqltxma.html

[S26] C：内存清零
来源：http://hz.jinqigufen.top/gtsfxgtyst.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gthubhojol.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtlnggynyv.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtdwpbijej.html

[S28] C：静态变量
来源：http://hz.xuanzx.com/gtcuzmmynl.html

static int counter = 0;
来源：http://hz.jyoumei.cn/gtzovimowy.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtiynvckte.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gtfpwmmvmf.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtmhpaalxa.html

#ifndef X_H
来源：http://hz.zhengqikj.top/gtupoiucxq.html

#define X_H
来源：http://hz.hammf.cn/gtofjmgokz.html

#endif
来源：http://hz.dashuyun.cn/gtgnlxlxhl.html

[S31] C++：Hello World
来源：http://hz.52xcode.cn/gtqziiafbo.html

#include <iostream>
来源：http://hz.fengsongda.top/gtashxozou.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ywan-chungtsiang.top/gtxemlhsse.html

[S32] C++：字符串
来源：http://hz.xinyue.icu/gtlkyhxtva.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtrgvktngv.html

[S33] C++：vector 增删
来源：http://hz.guowangkeji.top/gtxnziokbw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gtefpugfwa.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gtauzadfyw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtdnxwtirz.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gtkudlcomg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gttyjdzloh.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtijisqwth.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtyfhopdxu.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtpdkphvnf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydjk.org.cn/gtkpvjruga.html

[S38] C++：排序
来源：http://hz.guannengcc.top/gtkyewzpuj.html

std::sort(v.begin(), v.end());
来源：http://hz.hysaishi.cn/gtyugavjvq.html

[S39] C++：自定义比较器排序
来源：http://hz.shuidangran.top/gtuthwhljj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtrkzlltgk.html

[S40] C++：查找元素
来源：http://hz.wangshuangyany.cn/gtnkghvuvb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.aizwys.cn/gtvypfzlzl.html

[S41] C++：类与构造函数
来源：http://hz.feifeiyinyue.top/gtxlivgpyt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guannengcc.top/gtdvsfbpem.html

[S42] C++：继承与虚函数
来源：http://hz.daxiang520.top/gtjeaolqsp.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtwtfwvepx.html

[S43] C++：智能指针
来源：http://hz.yuanzhike.top/gthsqaxxei.html

auto p = std::make_unique<int>(5);
来源：http://hz.xylfe.cn/gtzeuqwtpl.html

[S44] C++：引用传参
来源：http://hz.ybcxt.top/gtuvgvufxz.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtcnhoeqaa.html

[S45] C++：lambda
来源：http://hz.cashguo.top/gtzkmryvqo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.svipenyu.cn/gtdpigzwfh.html

[S46] C++：函数模板
来源：http://hz.sxryk.cn/gtbasgelsc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yanxiufei.cn/gtrqparzgr.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258.top/gtuwudwsmw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.redwolf501.top/gtvbgaeezo.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtejkxfjyc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtldomfgph.html

while (std::getline(in, line)) { }
来源：http://hz.feifeiyinyue.top/gtvjrhaoph.html

[S49] C++：写文件
来源：http://hz.yueranfly.top/gtzavnnwgd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.feifeiyinyue.top/gtmrexnqcs.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtijveogeb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.iojbl.cn/gteadutlue.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtyowxbeca.html

static_cast<double>(a) / b
来源：http://hz.ywan-chungtsiang.top/gtsilncwmk.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtyvktuyve.html

int size() const noexcept { return n_; }
来源：http://hz.hywenlv.cn/gtmpzspkfl.html

[S53] C++：移动语义
来源：http://hz.sweek.top/gtnkqpcnpz.html

std::vector<int> w = std::move(v);
来源：http://hz.cdnleiting.top/gtmmvmiobw.html

[S54] C++：异常处理
来源：http://hz.zhoulong.xyz/gtbtsmljyb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.vqdsnc.cn/gtogwpmcug.html

[S55] C++：结构化绑定
来源：http://hz.dianchejie.cn/gtdnbfiqhj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gtyubjpnoi.html

[S56] C++：optional
来源：http://hz.ydzc1.top/gtozqjxkvy.html


<!-- 参考信息 -->