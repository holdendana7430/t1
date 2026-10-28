代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.52xcode.cn/gtvxppcsjj.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258888.top/gtqrjkfpzj.html

[Q85] 数值取整
来源：http://hz.quarkkingdee.top/gtdpjpzdnb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jianghu66.top/gtzjnusonw.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigufen.top/gtdgqrpqpe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhoulong.xyz/gtfiszjkks.html

[Q87] JSON 字段做条件
来源：http://hz.sxryk.cn/gttvddzzic.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dianchejie.cn/gtyppgngqn.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtoulmuzgi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hywenlv.cn/gtnrqgkjja.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangkeji.top/gtucomitfg.html

[Q89] 判断表是否存在
来源：http://hz.chenlongwang.top/gtazxlhgqv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangtech.top/gtktisumqd.html

[Q90] 生成序号列
来源：http://hz.gaohongyu789.top/gtmaeuupdk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ivvv.top/gtyehqbquh.html

================================================================================
来源：http://hz.chenzaomai.com/gtgruifmez.html

R. Bash 专题
来源：http://hz.shanyushiyangkeji.top/gtsanfhehq.html

================================================================================
来源：http://hz.svipenyu.cn/gtuehwrphv.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gtztyvttmj.html

#!/usr/bin/env bash
来源：http://hz.jinghuilouyu.cn/gtmhykkmfe.html

set -euo pipefail
来源：http://hz.zhijiandao.cn/gtgkrkunen.html

[R02] 变量赋值与使用
来源：http://hz.sysykeji.top/gtsnlspvsf.html

name="Tom"; echo "$name"
来源：http://hz.dianchejie.cn/gtdrnhlgcz.html

[R03] 只读变量
来源：http://hz.haohaochexian.top/gtaesjezhg.html

readonly PI=3.14
来源：http://hz.sweek.top/gtzizvovrf.html

[R04] 位置参数
来源：http://hz.birdmap.top/gtipoeazjr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.svipenyu.cn/gtmtkkfhdp.html

[R05] 参数默认值
来源：http://hz.zhengqikj.top/gtzyzhlzkm.html

name="${1:-default}"
来源：http://hz.hammf.cn/gtwwslobzx.html

[R06] 判断命令是否存在
来源：http://hz.sweek.top/gtwmpxkgvt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gtvbqpmjty.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtdgjurlhw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aibaodan.cn/gtohcmuryv.html

[R08] 数值比较
来源：http://hz.tianlin.xyz/gtpvjtcdnf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.meibo888.top/gtnsjudzmv.html

[R09] 字符串比较
来源：http://hz.52xcode.cn/gtjcnapozq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinghuilouyu.cn/gtwmcqoafb.html

[R10] 正则匹配
来源：http://hz.yueranfly.top/gtuubexqhm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gzhubu.top/gtecrtrdio.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtnuvzlolm.html

case "$1" in
来源：http://hz.bjfxy.top/gtlepjrhvw.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangtech.top/gthrlqdxqj.html

stop)  echo "停止" ;;
来源：http://hz.yj20258.top/gtndvtmapo.html

*)     echo "未知命令" ;;
来源：http://hz.gogol.net.cn/gtjhgntqrw.html

esac
来源：http://hz.jinqigfzy.top/gtzefwujbd.html

[R12] for 遍历文件
来源：http://hz.gaohongyu789.top/gtvjqfcgwn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xylfe.cn/gtiybazaya.html

[R13] for 计数循环
来源：http://hz.snrcjt.cn/gtgaqdpzxi.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fengsongda.top/gtgpwxrzvh.html

[R14] C 风格 for
来源：http://hz.sweek.top/gtnfjsbqgy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.mhx1999.top/gtfnfsczxi.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gthpkilazy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj202588.top/gttlpfhbvy.html

[R16] until 等待条件
来源：http://hz.hnxiangtu.top/gtzvmbasxs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtzreszuzj.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gtksrofvap.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hammf.cn/gttxevrzhb.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtkaqkcvit.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cashguo.top/gthpnnmzhs.html

[R19] 数组长度
来源：http://hz.yj202588.top/gtfpzzlama.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtfixekznz.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtupipzshk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yanxiufei.cn/gtjomsnizm.html

[R21] 字符串长度
来源：http://hz.jinyuanbaomall.cn/gtpjsxnrii.html

echo "${#s}"
来源：http://hz.shangyingyoupin.top/gttzddwsbh.html

[R22] 截取子串
来源：http://hz.daria6918.cn/gtlbjplotu.html

echo "${s:0:5}"
来源：http://hz.chenlongwang.top/gtukvaersv.html

[R23] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtgjewxcyd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pengpengdd.cyou/gtdwgmhgmt.html

[R24] 大小写转换
来源：http://hz.jlsjyb.cn/gtdbvjtrdz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zycfv.cn/gtprtqrdxl.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhaomingkeji.xyz/gtdncjkxts.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cashguo.top/gtsdorhuqc.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtqjfiensa.html

now=$(date +%F); echo "$now"
来源：http://hz.gaohongyu789.top/gtdriaabws.html

[R27] 算术展开
来源：http://hz.52xcode.cn/gtvyzoenmu.html

echo $((1 + 2 * 3))
来源：http://hz.zhongyouzk.top/gtsvmahuiv.html

[R28] 浮点运算
来源：http://hz.gogol.net.cn/gtwmvepowm.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj20258888.top/gtnnzkkgpn.html

[R29] 定义函数
来源：http://hz.shangyingyoupin.top/gtyxwzshok.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tianlin.xyz/gtdbriooqj.html

[R30] 函数返回状态码
来源：http://hz.jiagoushi.top/gtohrquqtr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtptaunyco.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gtiesdsroo.html

f() { local x=1; echo "$x"; }
来源：http://hz.feifeiyinyue.top/gtxigyblzt.html

[R32] 参数个数校验
来源：http://hz.yuanzhike.top/gtikbmxmls.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtdwncsxwq.html

[R33] 捕获错误并提示行号
来源：http://hz.shangyingyoupin.top/gtstwufyzq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydjk.org.cn/gtxxsybmit.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gtwcczugiz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtsskosgbr.html

[R35] 后台执行并等待
来源：http://hz.jqgfzy.top/gtuyftvuxh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtfxlkrudm.html

[R36] 并发执行多个任务
来源：http://hz.gogol.net.cn/gtdnsckhvk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gtxmqcccrb.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gtgkjestzd.html

files=$(ls -1)
来源：http://hz.yj20258888.top/gtohnhufjz.html

[R38] 管道串联
来源：http://hz.yuxming.cn/gtkveaexot.html

cat a.txt | grep -i error | wc -l
来源：http://hz.birdmap.top/gtoqxaqjis.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gtisqqgtqd.html

cmd > out.log 2>&1
来源：http://hz.zhiwuduotai.top/gtmngvffet.html

[R40] 追加写日志
来源：http://hz.haohaochexian.top/gtllvcgoxk.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtkzfsgpwd.html

[R41] 丢弃输出
来源：http://hz.tanke756.top/gtbfhadlny.html

cmd >/dev/null 2>&1
来源：http://hz.fzhhl.top/gtmnahzlov.html

[R42] 输入重定向
来源：http://hz.xziqi.cn/gtdykcskrh.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtazchlytc.html

[R43] 按名字查找文件
来源：http://hz.yuxming.cn/gtbzcjkxzr.html

find . -name "*.log" -type f
来源：http://hz.andypj.xyz/gtqibvbhuu.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gtneasjbwj.html

find . -mtime -7 -type f
来源：http://hz.zdqjudy.top/gtzxnynjzr.html

[R45] 批量删除
来源：http://hz.gzhubu.top/gtulzdgzfy.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gttnihqslo.html

[R46] 递归替换文件内容
来源：http://hz.chenjidiqi.icu/gttmopjzfa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtfvtupzfa.html

[R47] sed 单行替换
来源：http://hz.smart0.xyz/gtiaviilzr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gthhmrnvjl.html

[R48] awk 取指定列
来源：http://hz.redwolf501.top/gtpitodybm.html

awk '{print $1, $3}' a.txt
来源：http://hz.jiagoushi.top/gtmethyjca.html

[R49] awk 带条件
来源：http://hz.nanxinkj.top/gtvmbvhebd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hammf.cn/gtvbgdyejt.html

[R50] awk 求和
来源：http://hz.ywan-chungtsiang.top/gttfmkpqsv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtovkkhhsz.html

[R51] 排序去重取前几
来源：http://hz.chenzaomai.com/gtdlbhkylk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinyuanbaomall.cn/gtqjkzabwp.html

[R52] 统计行数
来源：http://hz.jianghu66.top/gtmtfcdrha.html

wc -l a.txt
来源：http://hz.cdnleiting.top/gttkkkzkwj.html

[R53] 查看文件头与实时尾
来源：http://hz.nwbrower.top/gtlctquvzb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hysaishi.cn/gtllnxagnj.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gttwaahhai.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gttcafnfnl.html

[R55] 压缩与解压
来源：http://hz.guowangkeji.top/gtcbhzvxum.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.feifeiyinyue.top/gtaisiwtxv.html

[R56] 远程拷贝
来源：http://hz.snrcjt.cn/gtilpqlyuy.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtamznkjqk.html

[R57] 远程执行命令
来源：http://hz.ybcxt.top/gtnkonlybx.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtbjwgkjrk.html

[R58] 下载文件
来源：http://hz.jqgfzy.top/gtigdmwgau.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gthyfuulzq.html

[R59] 发 POST JSON
来源：http://hz.gaohongyu789.top/gtsvpzmjmy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gtxyytluvl.html

[R60] 只看 HTTP 状态码
来源：http://hz.cdnleiting.top/gtohtyxgmd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.52xcode.cn/gtsnzulhal.html

[R61] 磁盘占用
来源：http://hz.nwbrower.top/gtsfxmnkbj.html

df -h;  du -sh *
来源：http://hz.yuanzhike.top/gtgegcxwfl.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtqzrxaoca.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gthdisdiox.html

[R63] 内存与进程
来源：http://hz.cqqwz.cn/gtlfebxmln.html

free -h;  ps aux | grep nginx
来源：http://hz.sufxvd.cn/gtbmgydtuz.html

[R64] 结束进程
来源：http://hz.zhongyouzk.top/gtuwokpggo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgufenzy.top/gtdkomgvim.html

[R65] 查看端口占用
来源：http://hz.jinqigfzy.top/gtjrkwowio.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangtech.top/gtsssbuwnj.html

[R66] 定时任务
来源：http://hz.aibaodan.cn/gtbzxdlkwn.html

crontab -e;  crontab -l
来源：http://hz.yj202588.top/gtrdjqhuut.html

[R67] 生成随机十六进制串
来源：http://hz.jianghu66.top/gtnchvgwvk.html

openssl rand -hex 16
来源：http://hz.shzxlz.cn/gtcddslhwk.html

[R68] 计算文件校验值
来源：http://hz.sxryk.cn/gtukjkpnwk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.c1oappe.top/gtvykzdbuj.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtfzxgyodc.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigfzy.top/gtyqjgeref.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtmxeqnawa.html

date +%s;  date -d @1700000000
来源：http://hz.jlsjyb.cn/gtaiiisbvn.html

[R71] 日期格式化
来源：http://hz.bjfxy.top/gtzcyjfdiz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxinkj.top/gtejaaenmq.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gtovmflpwp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.mhx1999.top/gtjectvmtr.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gtyhuvohff.html

split -l 1000 big.log part_
来源：http://hz.gzhubu.top/gtkxoeurwq.html

[R74] 批量重命名
来源：http://hz.cqqwz.cn/gtknomppyh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuanzx.com/gtpimfznjt.html

[R75] 导出环境变量
来源：http://hz.ydzc1.top/gtallaxzdq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangshuangyany.cn/gtcgqjpymi.html

[R76] 使用临时文件
来源：http://hz.zhongyouzk.top/gtccbvdack.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gtbmbfmyvo.html

[R77] 读取用户输入
来源：http://hz.svipenyu.cn/gtfoybilwu.html

read -rp "请输入: " ans
来源：http://hz.yj20258.top/gtongbfsbe.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gtrigcqbqp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtlzbkjcxq.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gthyednpby.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangkeji.top/gtsusvdiqq.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtysskujkg.html

time ./run.sh
来源：http://hz.jinqigufen.top/gtniutgyxd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgpbqqmxb.html

S. C / C++ 专题
来源：http://hz.zhiwuduotai.top/gtecplwvro.html

================================================================================
来源：http://hz.pycfn.com/gtaqddehxt.html

[S01] C：Hello World
来源：http://hz.yj202588.top/gteluyvrjg.html

#include <stdio.h>
来源：http://hz.ivvv.top/gtxhtqzbun.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtxaputswu.html

[S02] C：变量与格式化输出
来源：http://hz.hysaishi.cn/gtypdnmshp.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangshuangyany.cn/gtcumvlqdy.html

[S03] C：读入整数
来源：http://hz.zhaomingkeji.xyz/gtkbfdfwkk.html

int x; scanf("%d", &x);
来源：http://hz.redwolf501.top/gtxcjsdghg.html

[S04] C：字符串复制
来源：http://hz.jinyuanbaomall.cn/gtoshepsdm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.c1oappe.top/gtpbxgswoi.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gtzyaffggg.html

strlen(s)
来源：http://hz.tianlin.xyz/gthxhaupci.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtvkxujccg.html

strcmp(a, b) == 0
来源：http://hz.tian-w.cn/gthfbgjmab.html

[S07] C：数组遍历求和
来源：http://hz.jqgufenzy.top/gtdixytthb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtpmdicakp.html

[S08] C：动态内存分配与释放
来源：http://hz.shuidangran.top/gtnhegvgoa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhiwuduotai.top/gtuoefozhy.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtarnxsngb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xylfe.cn/gthjfkjiap.html

[S10] C：指针与解引用
来源：http://hz.jlsjyb.cn/gtqbaxufpv.html

int *p = &a;  *p = 5;
来源：http://hz.chenzaomai.com/gtdnvvwpdu.html

[S11] C：逐行读文件
来源：http://hz.aibaodan.cn/gtqzpkclzo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.snrcjt.cn/gteabaxwgx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hysaishi.cn/gtigujizbu.html

fclose(f);
来源：http://hz.c1oappe.top/gtvobahdnv.html

[S12] C：写文件
来源：http://hz.xziqi.cn/gttqknzfdi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.dianchejie.cn/gtbstytiju.html

[S13] C：宏定义
来源：http://hz.fzhhl.top/gtglpaesmh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hammf.cn/gtmszrkcsp.html

[S14] C：枚举
来源：http://hz.feifeiyinyue.top/gtoljjrdos.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinghuilouyu.cn/gtpxkpyywr.html

[S15] C：类型转换
来源：http://hz.xziqi.cn/gtmuzdgcio.html

(double) a / b
来源：http://hz.jinghuilouyu.cn/gtwwgcxfqw.html

[S16] C：位操作置位
来源：http://hz.jqgfzy.top/gttimnpsus.html

x |= (1 << 3);
来源：http://hz.fzhhl.top/gtullnybqi.html

[S17] C：安全拼接字符串
来源：http://hz.xylfe.cn/gtnfbzhmss.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gogol.net.cn/gtwprvnaph.html

[S18] C：命令行参数
来源：http://hz.hongshengwenyu.top/gtqkybsxzw.html

int main(int argc, char **argv)
来源：http://hz.yueranfly.top/gtriyyhllz.html

[S19] C：快速排序
来源：http://hz.cashguo.top/gtkuxzfyxg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xuanzx.com/gtftoxwtzv.html

[S20] C：二分查找
来源：http://hz.vqdsnc.cn/gtidkesqpr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtmdizbymx.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtciwevpyl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zycfv.cn/gtrqgazclr.html

[S22] C：字符串转数字
来源：http://hz.jqgfzy.top/gtwsgbrrtl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtsifaltca.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtkolmunnd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yangfankeji.com/gtvmjyezir.html

[S24] C：获取本地时间
来源：http://hz.aibaodan.cn/gtbyttydxz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guowangkeji.top/gtwtmzlpsd.html

[S25] C：内存拷贝
来源：http://hz.zhoulong.xyz/gthdbuflyy.html

memcpy(dst, src, n);
来源：http://hz.yuxming.cn/gtguyapktz.html

[S26] C：内存清零
来源：http://hz.chenzaomai.com/gtxfcnlrhw.html

memset(a, 0, sizeof a);
来源：http://hz.cheryme.top/gtrxzdpgql.html

[S27] C：定义常量
来源：http://hz.andypj.xyz/gtmgdmapas.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtsufosxeh.html

[S28] C：静态变量
来源：http://hz.zycfv.cn/gtuarnnovt.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtlxsycskg.html

[S29] C：变参函数
来源：http://hz.zhengqikj.top/gthcxsjtte.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gthpgoavmt.html

[S30] C：头文件保护
来源：http://hz.fzhhl.top/gtgrhatuuv.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtrrybteyh.html

#define X_H
来源：http://hz.yj202588.top/gtteqgeyux.html

#endif
来源：http://hz.zhijiandao.cn/gtqdhvumnw.html

[S31] C++：Hello World
来源：http://hz.zhoulong.xyz/gtiszaaeat.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtimfxrbro.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gzhubu.top/gtzkuoqtbr.html

[S32] C++：字符串
来源：http://hz.havefunace.top/gtvvowlxek.html

std::string s = "hi";  s += "!";
来源：http://hz.gaohongyu789.top/gtnoancrdv.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtcoucumsh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtmtgqscmb.html

[S34] C++：遍历 vector
来源：http://hz.aizwys.cn/gtpwlzvzhx.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jiagoushi.top/gtgcnogzyc.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gtschnjbob.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.vqdsnc.cn/gtfueqctcm.html

[S36] C++：unordered_map
来源：http://hz.jyoumei.cn/gtfbxfsujt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtnnuhrtpm.html

[S37] C++：set
来源：http://hz.sxryk.cn/gtavmmyflh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuanzhike.top/gtlftigggi.html

[S38] C++：排序
来源：http://hz.kuanghao11.cn/gtigjehcur.html

std::sort(v.begin(), v.end());
来源：http://hz.jlsjyb.cn/gtrambvwas.html

[S39] C++：自定义比较器排序
来源：http://hz.xingfuxueyuan.xyz/gtemmprdin.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sufxvd.cn/gtomoryeiq.html

[S40] C++：查找元素
来源：http://hz.aibaodan.cn/gtbdzbbqak.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zdqjudy.top/gthkuzbaou.html

[S41] C++：类与构造函数
来源：http://hz.quarkkingdee.top/gtorfwcjdg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.snrcjt.cn/gtumgfdsar.html

[S42] C++：继承与虚函数
来源：http://hz.52xcode.cn/gtcfbskykr.html

class B : public Base { public: void f() override {} };
来源：http://hz.yangfankeji.com/gtqqvmrccq.html

[S43] C++：智能指针
来源：http://hz.jlsjyb.cn/gthkrpwwqp.html

auto p = std::make_unique<int>(5);
来源：http://hz.hywenlv.cn/gttfyerbaw.html

[S44] C++：引用传参
来源：http://hz.yj202588.top/gtdydiixmz.html

void inc(int &x) { ++x; }
来源：http://hz.ehwqpu.com/gtwxfqnzig.html

[S45] C++：lambda
来源：http://hz.hongshengwenyu.top/gtpxbbxmng.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenlongwang.top/gtzlevuhty.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gttrcwxrgt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yangfankeji.com/gtvoqqpslm.html

[S47] C++：结构化绑定遍历
来源：http://hz.fengsongda.top/gtxhggxani.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtutpwytzh.html

[S48] C++：逐行读文件
来源：http://hz.hywenlv.cn/gttsxgzhxy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtxaxwfvdf.html

while (std::getline(in, line)) { }
来源：http://hz.havefunace.top/gtdtxwtggd.html

[S49] C++：写文件
来源：http://hz.yangfankeji.com/gtskhfupju.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.vqdsnc.cn/gtflhyjwns.html

[S50] C++：格式化数字
来源：http://hz.xuanzx.com/gtutzgjavu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tianlin.xyz/gtmcnzgbrk.html

[S51] C++：显式类型转换
来源：http://hz.yj202588.top/gtyzbnodol.html

static_cast<double>(a) / b
来源：http://hz.chenlongwang.top/gtchdcgqwf.html

[S52] C++：const 与 noexcept
来源：http://hz.ehwqpu.com/gtitbjkehy.html

int size() const noexcept { return n_; }
来源：http://hz.yvedp.cn/gtlaiddzfe.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangkeji.top/gtrlqvonzw.html

std::vector<int> w = std::move(v);
来源：http://hz.shanyushiyangkeji.top/gtyqwlfjtr.html

[S54] C++：异常处理
来源：http://hz.jinqigfzy.top/gtxcsbwpwz.html


<!-- 参考信息 -->