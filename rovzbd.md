代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtgnnmzpco.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gtusuujcif.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtrpsvnmry.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xinyue.icu/gtfqzekqus.html

[Q84] 去除首尾空格
来源：http://hz.shzxlz.cn/gtpfjguhjh.html

SELECT TRIM(name) FROM users;
来源：http://hz.tian-w.cn/gtelkfjuwq.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtolfivesr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.snrcjt.cn/gtzxgosbxg.html

[Q86] 读取 JSON 字段
来源：http://hz.sysykeji.top/gtjmcqhtqm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhixingplan.top/gtzdxtckrh.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gttdvaocou.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jyoumei.cn/gttxdcrnlm.html

[Q88] 行转列（条件聚合）
来源：http://hz.shanyushiyangtech.top/gtoyclcviv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yanxiufei.cn/gtbvqlzbbw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cucudq.cn/gtjjzmhamm.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtjzxumuqs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtfhrfpgut.html

[Q90] 生成序号列
来源：http://hz.daria6918.cn/gtkfhyncdu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydjk.org.cn/gtzilmikjl.html

================================================================================
来源：http://hz.aibaodan.cn/gteybuadvz.html

R. Bash 专题
来源：http://hz.sysykeji.top/gtsmpwglgq.html

================================================================================
来源：http://hz.tanke756.top/gtivbwrqlp.html

[R01] shebang 与严格模式
来源：http://hz.dianchejie.cn/gtlokohsbe.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtkstzjibg.html

set -euo pipefail
来源：http://hz.sufxvd.cn/gtjlgsagzv.html

[R02] 变量赋值与使用
来源：http://hz.kuanghao11.cn/gtxrugmfrt.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtitlyjdlf.html

[R03] 只读变量
来源：http://hz.hnqzz.top/gtpubrtunw.html

readonly PI=3.14
来源：http://hz.sufxvd.cn/gtwmxndcds.html

[R04] 位置参数
来源：http://hz.mhx1999.top/gtatbxoaak.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.gzhubu.top/gtmawybmsi.html

[R05] 参数默认值
来源：http://hz.shanyushiyangtech.top/gtughjuhsj.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtxbebbsru.html

[R06] 判断命令是否存在
来源：http://hz.yj202588.top/gtmdmjfbjq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dashuyun.cn/gtguijpeha.html

[R07] if 判断文件
来源：http://hz.yueranfly.top/gtloyiuzvz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tian-w.cn/gtmodiltmv.html

[R08] 数值比较
来源：http://hz.hongshengwenyu.top/gttnifncbg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuxming.cn/gtzuvifbkp.html

[R09] 字符串比较
来源：http://hz.nanxinkj.top/gtvviemxvk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gogol.net.cn/gtkhbsotat.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtpviaxxob.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtblcosruh.html

[R11] case 多分支
来源：http://hz.aizwys.cn/gtbvtlaxux.html

case "$1" in
来源：http://hz.aizwys.cn/gtuncdfmlr.html

start) echo "启动" ;;
来源：http://hz.hywenlv.cn/gtvfqwofgq.html

stop)  echo "停止" ;;
来源：http://hz.guannengcc.top/gtwhlskbww.html

*)     echo "未知命令" ;;
来源：http://hz.andypj.xyz/gtrbjuiryv.html

esac
来源：http://hz.yueranfly.top/gtydjpeoyj.html

[R12] for 遍历文件
来源：http://hz.hnxiangtu.top/gtiowdmmkf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shzxlz.cn/gttvvbgdox.html

[R13] for 计数循环
来源：http://hz.xziqi.cn/gtrrsoipig.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtkjwvwqjk.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtbbymcgjk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtplcnxolp.html

[R15] while 逐行读文件
来源：http://hz.xuetiantiany.cn/gtvchpkkox.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtdgtvewdk.html

[R16] until 等待条件
来源：http://hz.snrcjt.cn/gtwzkoyboq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cashguo.top/gtqrwvjirc.html

[R17] 数组定义与取值
来源：http://hz.ydzc1.top/gtctxhrtcx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cashguo.top/gthsbiaqqx.html

[R18] 遍历数组
来源：http://hz.pengpengdd.cyou/gtggwcygji.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtpdqxdefd.html

[R19] 数组长度
来源：http://hz.tian-w.cn/gtoezriemy.html

echo "${#arr[@]}"
来源：http://hz.cheryme.top/gtcuhcotcf.html

[R20] 关联数组（字典）
来源：http://hz.yuxming.cn/gtitplmsrk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangdashe.top/gtnzwcruvj.html

[R21] 字符串长度
来源：http://hz.hnqzz.top/gtxtspvyll.html

echo "${#s}"
来源：http://hz.yj20258888.top/gtkkdhgccf.html

[R22] 截取子串
来源：http://hz.wangshuangyany.cn/gtgtbqjstl.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtgtahzgwq.html

[R23] 字符串替换
来源：http://hz.hysaishi.cn/gtlnafbdkj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.316326.xyz/gtgakhdvgu.html

[R24] 大小写转换
来源：http://hz.hywenlv.cn/gthqsawizl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tanke756.top/gtwukhjimk.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtngaggrfz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtgrqcodys.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtyvemipkv.html

now=$(date +%F); echo "$now"
来源：http://hz.gotoacloud.top/gtfvcjymkg.html

[R27] 算术展开
来源：http://hz.xingfuxueyuan.xyz/gtbesazako.html

echo $((1 + 2 * 3))
来源：http://hz.yueranfly.top/gtvtoijwpj.html

[R28] 浮点运算
来源：http://hz.kuanghao11.cn/gtrhtigoug.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenzaomai.com/gtfijmlsvj.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtwbeaxcte.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangshuangyany.cn/gtzfrbzrgh.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtksogmxau.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xylfe.cn/gtfzlpcnwo.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gteuzusccj.html

f() { local x=1; echo "$x"; }
来源：http://hz.andypj.xyz/gtoacevawg.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtbukpeiyy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydzc1.top/gtcblngbcn.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtxqbfoxgl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuanzhike.top/gtymssohfo.html

[R34] 退出时清理
来源：http://hz.svipenyu.cn/gtrmxhjonk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydzc1.top/gttvsxnsho.html

[R35] 后台执行并等待
来源：http://hz.hnqzz.top/gtekobeoys.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuanzx.com/gtsgdmvoon.html

[R36] 并发执行多个任务
来源：http://hz.ivvv.top/gtbslhnmil.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shzxlz.cn/gtjaohogtf.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gtvibfhhey.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtfcugijgt.html

[R38] 管道串联
来源：http://hz.zycfv.cn/gtzbfscnlb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtzwaoygxi.html

[R39] 重定向标准输出与错误
来源：http://hz.zhaomingkeji.xyz/gtovbwawyk.html

cmd > out.log 2>&1
来源：http://hz.mhx1999.top/gtrmaqkuxu.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gteblohnps.html

echo "log" >> out.log
来源：http://hz.snrcjt.cn/gtgmhikrpg.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtutzwnnpy.html

cmd >/dev/null 2>&1
来源：http://hz.nanxuanxn.top/gtvhyfejqn.html

[R42] 输入重定向
来源：http://hz.zhoulong.xyz/gtdsropldm.html

wc -l < a.txt
来源：http://hz.yonumen.top/gtuslzetkh.html

[R43] 按名字查找文件
来源：http://hz.feifeiyinyue.top/gtjhpvobxk.html

find . -name "*.log" -type f
来源：http://hz.jlsjyb.cn/gtfuzcrjnn.html

[R44] 按修改时间查找
来源：http://hz.wangshuangyany.cn/gtmmgkshnk.html

find . -mtime -7 -type f
来源：http://hz.yj20258.top/gttxafrpwp.html

[R45] 批量删除
来源：http://hz.yanxiufei.cn/gtfkgvtomd.html

find . -name "*.tmp" -delete
来源：http://hz.shangyingyoupin.top/gtimbbhack.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gtrudkrwzh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sysykeji.top/gtcurccygu.html

[R47] sed 单行替换
来源：http://hz.hongshengwenyu.top/gtahmjcacm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tianlin.xyz/gtrimokvmi.html

[R48] awk 取指定列
来源：http://hz.jiagoushi.top/gtcxbkaphw.html

awk '{print $1, $3}' a.txt
来源：http://hz.hfpthk.cn/gtppgvjati.html

[R49] awk 带条件
来源：http://hz.jinghuilouyu.cn/gtyakvknio.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.svipenyu.cn/gtclsojbdz.html

[R50] awk 求和
来源：http://hz.guannengcc.top/gtdoapfbwg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtkswwithk.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtvotgulpg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pengpengdd.cyou/gtfclrazdu.html

[R52] 统计行数
来源：http://hz.yvedp.cn/gtiiibqnqs.html

wc -l a.txt
来源：http://hz.chenjidiqi.icu/gtzwxvbhqm.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gthvrejmac.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangdashe.top/gtdkthvmve.html

[R54] 比较两个文件
来源：http://hz.wangdashe.top/gtnoddatti.html

diff a.txt b.txt
来源：http://hz.xuetiantiany.cn/gtvrdlxsuc.html

[R55] 压缩与解压
来源：http://hz.chenjidiqi.icu/gtggkvhdkc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pengpengdd.cyou/gtdnpkojcz.html

[R56] 远程拷贝
来源：http://hz.chenlongwang.top/gtvghxfenr.html

scp file user@host:/path/
来源：http://hz.cdnleiting.top/gtozbxigqo.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtjgqfhqea.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtrqmvwzeo.html

[R58] 下载文件
来源：http://hz.zhaomingkeji.xyz/gttnfjpqzn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenlongwang.top/gtidcqdond.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtugxgaxrb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtincwnyim.html

[R60] 只看 HTTP 状态码
来源：http://hz.andypj.xyz/gtkxckyzwn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.bjfxy.top/gtencdvsux.html

[R61] 磁盘占用
来源：http://hz.yongpay.top/gtypxpcsbj.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtirpaflvk.html

[R62] 找最占空间的文件
来源：http://hz.chenjidiqi.icu/gtnvwcymsq.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtulackpbx.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtpmwckjli.html

free -h;  ps aux | grep nginx
来源：http://hz.aibaodan.cn/gtaxmtedva.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtariryoca.html

kill -9 $(pgrep -f app.py)
来源：http://hz.smart0.xyz/gtglzycxfc.html

[R65] 查看端口占用
来源：http://hz.jianghu66.top/gtjeygkpfx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jiagoushi.top/gtvdhkbzap.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtfptermxo.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtyppospok.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtpuhkdrfc.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gtjhfqnvnb.html

[R68] 计算文件校验值
来源：http://hz.xuanzx.com/gtxsejytwo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnxiangtu.top/gtgnbhpntc.html

[R69] 生成随机密码
来源：http://hz.guowangkeji.top/gtekafoeig.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gttxjikmqy.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtzqcrchak.html

date +%s;  date -d @1700000000
来源：http://hz.xuanzx.com/gttdgnrndf.html

[R71] 日期格式化
来源：http://hz.mhx1999.top/gtcbyvjgxv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guowangkeji.top/gtekzwnjfz.html

[R72] 等待端口就绪
来源：http://hz.cdnleiting.top/gtfxzemnbm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtlvfnniib.html

[R73] 分割大日志
来源：http://hz.xylfe.cn/gtqtikrllj.html

split -l 1000 big.log part_
来源：http://hz.yongpay.top/gtfbypxjvb.html

[R74] 批量重命名
来源：http://hz.shanyushiyangkeji.top/gtlbarnmij.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigufen.top/gtrjucivxr.html

[R75] 导出环境变量
来源：http://hz.wangshuangyany.cn/gtcqkpdjqw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.andypj.xyz/gtrjowyysq.html

[R76] 使用临时文件
来源：http://hz.chenlongwang.top/gtqhijsvzv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtxmsaksip.html

[R77] 读取用户输入
来源：http://hz.iojbl.cn/gtlpjgjksu.html

read -rp "请输入: " ans
来源：http://hz.yvedp.cn/gtumfducvu.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtutucohps.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shzxlz.cn/gtiydaxdoy.html

[R79] 解析命令行选项
来源：http://hz.andypj.xyz/gtjjeppsze.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sufxvd.cn/gtszjzftdu.html

[R80] 查看脚本执行耗时
来源：http://hz.zhixingplan.top/gtcryedwhe.html

time ./run.sh
来源：http://hz.jinqigufen.top/gtqbphsasz.html

================================================================================
来源：http://hz.havefunace.top/gtqrccshtp.html

S. C / C++ 专题
来源：http://hz.gaohongyu789.top/gtqhuvgkhe.html

================================================================================
来源：http://hz.sxryk.cn/gtsojcllhe.html

[S01] C：Hello World
来源：http://hz.yuanzhike.top/gtltvgedzy.html

#include <stdio.h>
来源：http://hz.xziqi.cn/gtksbmwkol.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258888.top/gtgcgbezmz.html

[S02] C：变量与格式化输出
来源：http://hz.quarkkingdee.top/gtonxmlqkn.html

int a = 10; printf("%d\n", a);
来源：http://hz.gogol.net.cn/gtqpqybifv.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtknnfqsnh.html

int x; scanf("%d", &x);
来源：http://hz.chenjidiqi.icu/gtnrqtvvrs.html

[S04] C：字符串复制
来源：http://hz.yuxming.cn/gtxarhqjlm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pengpengdd.cyou/gtixswmhzs.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtvzwyzlgm.html

strlen(s)
来源：http://hz.daxiang520.top/gthjkibslg.html

[S06] C：字符串比较
来源：http://hz.nanxuanxn.top/gtrwxuozmm.html

strcmp(a, b) == 0
来源：http://hz.tian-w.cn/gtjkiwjpnk.html

[S07] C：数组遍历求和
来源：http://hz.meibo888.top/gtgkwmbywh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtljdnsswc.html

[S08] C：动态内存分配与释放
来源：http://hz.gotoacloud.top/gtonhdwalu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yanxiufei.cn/gtvrwhnujq.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258.top/gthousgnnj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtbnmozcbe.html

[S10] C：指针与解引用
来源：http://hz.daria6918.cn/gtkcywplvz.html

int *p = &a;  *p = 5;
来源：http://hz.wangdashe.top/gttaysddkx.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtoutepyit.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gtpvwvhhub.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hongshengwenyu.top/gtjdkkgvjs.html

fclose(f);
来源：http://hz.jinghuilouyu.cn/gtnwzjgcgh.html

[S12] C：写文件
来源：http://hz.daxiang520.top/gtlbxtthkg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgufenzy.top/gtkunxnewx.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtxbbojvwg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydjk.org.cn/gtxrwdlpjk.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtegwvjzni.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zycfv.cn/gtehxbiuaa.html

[S15] C：类型转换
来源：http://hz.dashuyun.cn/gtfemvxjwo.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtvhixcwyp.html

[S16] C：位操作置位
来源：http://hz.cheryme.top/gtgyoougdn.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gtpeosneaj.html

[S17] C：安全拼接字符串
来源：http://hz.yueranfly.top/gtzxiunvnv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gtycwuuerh.html

[S18] C：命令行参数
来源：http://hz.yanxiufei.cn/gtsscmxors.html

int main(int argc, char **argv)
来源：http://hz.snrcjt.cn/gtesicqkgx.html

[S19] C：快速排序
来源：http://hz.ybcxt.top/gtzwaivsdu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtnsynpims.html

[S20] C：二分查找
来源：http://hz.haohaochexian.top/gthuxifyyq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sysykeji.top/gtujtcdste.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtjvznspgl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sweek.top/gtuhaiwkah.html

[S22] C：字符串转数字
来源：http://hz.jinghuilouyu.cn/gtfwccewyn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.meibo888.top/gtaxnmhekg.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gttrywgnlc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daria6918.cn/gtsztkrsqx.html

[S24] C：获取本地时间
来源：http://hz.havefunace.top/gtnphljpak.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.snrcjt.cn/gtsirqwefb.html

[S25] C：内存拷贝
来源：http://hz.ivvv.top/gtssmacjzp.html

memcpy(dst, src, n);
来源：http://hz.chenlongwang.top/gttxckeofq.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtjmqbfify.html

memset(a, 0, sizeof a);
来源：http://hz.aizwys.cn/gtapfuyheq.html

[S27] C：定义常量
来源：http://hz.yj20258.top/gtneeqvtgn.html

const double PI = 3.14159;
来源：http://hz.yueranfly.top/gtxporltrd.html

[S28] C：静态变量
来源：http://hz.chenlongwang.top/gtmhmcwiat.html

static int counter = 0;
来源：http://hz.ydzc1.top/gtlzyihwnu.html

[S29] C：变参函数
来源：http://hz.hongshengwenyu.top/gtgoksorqt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydzc1.top/gtkxpiwpfb.html

[S30] C：头文件保护
来源：http://hz.shzxlz.cn/gtvmnffzwd.html

#ifndef X_H
来源：http://hz.jyoumei.cn/gtoueuhhds.html

#define X_H
来源：http://hz.nanxinkj.top/gtgvkiylex.html

#endif
来源：http://hz.shuidangran.top/gtlnnnvzef.html

[S31] C++：Hello World
来源：http://hz.vqdsnc.cn/gtynmrtsrg.html

#include <iostream>
来源：http://hz.ydzc1.top/gtykqzouux.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ppjwa.cn/gtqiejrfzq.html

[S32] C++：字符串
来源：http://hz.tianlin.xyz/gtcujkmsea.html

std::string s = "hi";  s += "!";
来源：http://hz.c1oappe.top/gtldzqktbo.html

[S33] C++：vector 增删
来源：http://hz.cdnleiting.top/gtwmfseiaa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ywan-chungtsiang.top/gtgnicahya.html

[S34] C++：遍历 vector
来源：http://hz.zhixingplan.top/gtcuregkuj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.feifeiyinyue.top/gtlzphzjjj.html

[S35] C++：map
来源：http://hz.zhongyouzk.top/gtffozmmis.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtznzkorhh.html

[S36] C++：unordered_map
来源：http://hz.cheryme.top/gtveetyaxd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtvghxgxnr.html

[S37] C++：set
来源：http://hz.gaohongyu789.top/gtjsmkzsrf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.52xcode.cn/gtunkgfmsg.html

[S38] C++：排序
来源：http://hz.hnqzz.top/gtrxvmgqyo.html

std::sort(v.begin(), v.end());
来源：http://hz.haohaochexian.top/gtpvosjufx.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtpmpgotue.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cucudq.cn/gtqitjjlio.html

[S40] C++：查找元素
来源：http://hz.shuidangran.top/gtjxykhwrm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.birdmap.top/gtckaojcrw.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gtatsjxapj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangdashe.top/gtvjwmpobq.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gtynslqbbd.html

class B : public Base { public: void f() override {} };
来源：http://hz.yangfankeji.com/gtvrteswso.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtigqgigew.html

auto p = std::make_unique<int>(5);
来源：http://hz.nwbrower.top/gtsdrrxhlh.html

[S44] C++：引用传参
来源：http://hz.snrcjt.cn/gtrxrvuary.html

void inc(int &x) { ++x; }
来源：http://hz.mhx1999.top/gtpewhetmn.html

[S45] C++：lambda
来源：http://hz.feifeiyinyue.top/gtfjcntqfp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sweek.top/gtakhlpgsm.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangtech.top/gttzlgxauf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtkkvriahi.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gtvhcfmwxe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.kuanghao11.cn/gtypfbcjnf.html

[S48] C++：逐行读文件
来源：http://hz.hnxiangtu.top/gthtlokirm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtkocxyzlj.html

while (std::getline(in, line)) { }
来源：http://hz.hnxiangtu.top/gthgudkdju.html

[S49] C++：写文件
来源：http://hz.fengsongda.top/gtzsyxnzct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gtkzplaxdh.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtnyqbjoej.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtcszgxqop.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gteibkllfl.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gtrntyohcy.html

[S52] C++：const 与 noexcept
来源：http://hz.xylfe.cn/gtrvtedzbl.html


<!-- 参考信息 -->