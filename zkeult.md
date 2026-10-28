代发 wailian999

[Q80] 字符串截取
来源：http://hz.52xcode.cn/gtkzhlfaoo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yvedp.cn/gtgbwdznxx.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gturkqeqtl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hammf.cn/gtfkumjcmi.html

[Q82] 字符长度与字节长度
来源：http://hz.yongpay.top/gtgbhmwtkp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guannengcc.top/gtfvarjhch.html

[Q83] 大小写转换
来源：http://hz.cqqwz.cn/gtxjshhkzi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtluclrybx.html

[Q84] 去除首尾空格
来源：http://hz.jqgfzy.top/gtuneguuwx.html

SELECT TRIM(name) FROM users;
来源：http://hz.cdnleiting.top/gtdnkkccno.html

[Q85] 数值取整
来源：http://hz.daria6918.cn/gtrydcntwe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtmtfjafxr.html

[Q86] 读取 JSON 字段
来源：http://hz.tianlin.xyz/gthunziiou.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.birdmap.top/gtaplggeok.html

[Q87] JSON 字段做条件
来源：http://hz.52xcode.cn/gtkgpcgvpx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shanyushiyangkeji.top/gtkjzhjsve.html

[Q88] 行转列（条件聚合）
来源：http://hz.daxiang520.top/gtoiuvyptb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangdashe.top/gtplznryei.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cucudq.cn/gthotfbcxx.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtdwdvbdzp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zycfv.cn/gtadkrraor.html

[Q90] 生成序号列
来源：http://hz.iojbl.cn/gtniekiiiz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenzaomai.com/gtbswxcvrt.html

================================================================================
来源：http://hz.dianchejie.cn/gtvaokknpa.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtckohmnjm.html

================================================================================
来源：http://hz.dianchejie.cn/gtzjffbonj.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gtwwlmtjxy.html

#!/usr/bin/env bash
来源：http://hz.guowangkeji.top/gtunvwpowc.html

set -euo pipefail
来源：http://hz.fengsongda.top/gtbrpjquza.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtzzuvhyoe.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtwvdlrfkc.html

[R03] 只读变量
来源：http://hz.tanke756.top/gtgiqrrpbs.html

readonly PI=3.14
来源：http://hz.hfpthk.cn/gtfxbjxxoy.html

[R04] 位置参数
来源：http://hz.c1oappe.top/gtvrcpoqkm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigufen.top/gtbyjkhtco.html

[R05] 参数默认值
来源：http://hz.shzxlz.cn/gthnhlzzyh.html

name="${1:-default}"
来源：http://hz.ehwqpu.com/gtqfkkztfg.html

[R06] 判断命令是否存在
来源：http://hz.xylfe.cn/gtiailnmft.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtcrypgppz.html

[R07] if 判断文件
来源：http://hz.zhiwuduotai.top/gtrgpajkct.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.snrcjt.cn/gthkrekwhb.html

[R08] 数值比较
来源：http://hz.sweek.top/gtechmtxlq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gotoacloud.top/gtmgwyyect.html

[R09] 字符串比较
来源：http://hz.ybcxt.top/gtslbzlzvm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtregtbzkx.html

[R10] 正则匹配
来源：http://hz.yj20258.top/gthnixotmj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yangfankeji.com/gtttekdyco.html

[R11] case 多分支
来源：http://hz.svipenyu.cn/gtobxasfkm.html

case "$1" in
来源：http://hz.xuanzx.com/gtelzickok.html

start) echo "启动" ;;
来源：http://hz.52xcode.cn/gtxzuuhayi.html

stop)  echo "停止" ;;
来源：http://hz.ivvv.top/gtjaczoadd.html

*)     echo "未知命令" ;;
来源：http://hz.yuxming.cn/gtsbrbigeo.html

esac
来源：http://hz.hfpthk.cn/gtctkipvie.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtmglvlzys.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtbyzthlma.html

[R13] for 计数循环
来源：http://hz.dianchejie.cn/gtwjuzcrwu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtwfvcyosg.html

[R14] C 风格 for
来源：http://hz.hammf.cn/gtsbbimsdh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtihaqzjwh.html

[R15] while 逐行读文件
来源：http://hz.xziqi.cn/gtcowkufyz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hnqzz.top/gtizhnpjjj.html

[R16] until 等待条件
来源：http://hz.mhx1999.top/gtekdfxtim.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenzaomai.com/gtjbykvaat.html

[R17] 数组定义与取值
来源：http://hz.xziqi.cn/gtgacchfki.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hfpthk.cn/gtzweqettt.html

[R18] 遍历数组
来源：http://hz.zhengqikj.top/gtvnohmwef.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nwbrower.top/gtpnuqxhzn.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtzmlzksaz.html

echo "${#arr[@]}"
来源：http://hz.shanyushiyangkeji.top/gtzkxysuyh.html

[R20] 关联数组（字典）
来源：http://hz.xuanzx.com/gtwmkrxhjp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuanzhike.top/gtouphgmtw.html

[R21] 字符串长度
来源：http://hz.hammf.cn/gtiaauhoek.html

echo "${#s}"
来源：http://hz.tanke756.top/gtzjynvgaz.html

[R22] 截取子串
来源：http://hz.fengsongda.top/gtutbbfuqc.html

echo "${s:0:5}"
来源：http://hz.cqqwz.cn/gtnjeoiqqj.html

[R23] 字符串替换
来源：http://hz.ydzc1.top/gtafrmozcm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.daxiang520.top/gttpznmmpm.html

[R24] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtqrkmkobi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hongshengwenyu.top/gtjplornzc.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxuanxn.top/gtybzdzrgb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hfpthk.cn/gtfizziawf.html

[R26] 命令替换
来源：http://hz.feifeiyinyue.top/gtiumhpsxp.html

now=$(date +%F); echo "$now"
来源：http://hz.ywan-chungtsiang.top/gtluxfhwxn.html

[R27] 算术展开
来源：http://hz.xylfe.cn/gtdycwiqkk.html

echo $((1 + 2 * 3))
来源：http://hz.aibaodan.cn/gtnpnrmtrx.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtebqtagpg.html

echo "scale=2; 10/3" | bc
来源：http://hz.sufxvd.cn/gtvzjzgxij.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtvzvtnwls.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gtnmjpefjq.html

[R30] 函数返回状态码
来源：http://hz.jqgfzy.top/gtccmnmpxg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tanke756.top/gtpinmegsf.html

[R31] 局部变量
来源：http://hz.cqqwz.cn/gtfptwsefl.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnqzz.top/gtiqenlnao.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtdzhtybta.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gzhubu.top/gtmipwojvx.html

[R33] 捕获错误并提示行号
来源：http://hz.hongshengwenyu.top/gttvpyobhm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtieofqaij.html

[R34] 退出时清理
来源：http://hz.nwbrower.top/gtibkbbyah.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtlbidditd.html

[R35] 后台执行并等待
来源：http://hz.sysykeji.top/gtgxlqjlzd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gtajgobjxm.html

[R36] 并发执行多个任务
来源：http://hz.pengpengdd.cyou/gtxnuhzxsg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.haohaochexian.top/gtpfvrxlyx.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtptmzokra.html

files=$(ls -1)
来源：http://hz.sxryk.cn/gtbzqhwnwh.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gtzjbrwyhg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shzxlz.cn/gtwduahgas.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtkenxahwx.html

cmd > out.log 2>&1
来源：http://hz.shuidangran.top/gtohxfwbyx.html

[R40] 追加写日志
来源：http://hz.hywenlv.cn/gthjikrlfg.html

echo "log" >> out.log
来源：http://hz.zhiwuduotai.top/gtmepmvwfr.html

[R41] 丢弃输出
来源：http://hz.xinyue.icu/gtgnfqsheo.html

cmd >/dev/null 2>&1
来源：http://hz.gzhubu.top/gtrbhweucp.html

[R42] 输入重定向
来源：http://hz.jinghuilouyu.cn/gtdcqzojxp.html

wc -l < a.txt
来源：http://hz.feifeiyinyue.top/gtdfhqiiup.html

[R43] 按名字查找文件
来源：http://hz.cheryme.top/gtzcwjspwe.html

find . -name "*.log" -type f
来源：http://hz.bjfxy.top/gtnceaekuj.html

[R44] 按修改时间查找
来源：http://hz.kuanghao11.cn/gtorpibfzm.html

find . -mtime -7 -type f
来源：http://hz.jqgufenzy.top/gtrzrqvpxx.html

[R45] 批量删除
来源：http://hz.52xcode.cn/gtgfpkifae.html

find . -name "*.tmp" -delete
来源：http://hz.yangfankeji.com/gtirrydfgl.html

[R46] 递归替换文件内容
来源：http://hz.aibaodan.cn/gtwdofidlo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gthkdycvil.html

[R47] sed 单行替换
来源：http://hz.meibo888.top/gtnjfxfumb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhixingplan.top/gtewstaffl.html

[R48] awk 取指定列
来源：http://hz.feifeiyinyue.top/gthddxvapx.html

awk '{print $1, $3}' a.txt
来源：http://hz.snrcjt.cn/gtrgxwfsoi.html

[R49] awk 带条件
来源：http://hz.hnxiangtu.top/gtiqprgqfw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenjidiqi.icu/gtobjzwvut.html

[R50] awk 求和
来源：http://hz.andypj.xyz/gtsqleqdql.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhengqikj.top/gtxqxatczn.html

[R51] 排序去重取前几
来源：http://hz.pengpengdd.cyou/gthhhwuiav.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ppjwa.cn/gtomflvuun.html

[R52] 统计行数
来源：http://hz.sysykeji.top/gtxpzlgufd.html

wc -l a.txt
来源：http://hz.bjfxy.top/gtxbewrbnl.html

[R53] 查看文件头与实时尾
来源：http://hz.nwbrower.top/gtzemzsfkf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtxfukcrar.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtdtuncvte.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtzxeqnxsq.html

[R55] 压缩与解压
来源：http://hz.hfpthk.cn/gtlmjaqcsb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenlongwang.top/gtlxfykpgz.html

[R56] 远程拷贝
来源：http://hz.chenzaomai.com/gtynywkifs.html

scp file user@host:/path/
来源：http://hz.jiagoushi.top/gthtnlpnpr.html

[R57] 远程执行命令
来源：http://hz.guowangkeji.top/gtwreuxkpg.html

ssh user@host 'uptime'
来源：http://hz.ydjk.org.cn/gtzqsqqaaw.html

[R58] 下载文件
来源：http://hz.ppjwa.cn/gtrhwzcjsr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtaxcobnej.html

[R59] 发 POST JSON
来源：http://hz.wangshuangyany.cn/gtvsooegzz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tianlin.xyz/gtskmeuupl.html

[R60] 只看 HTTP 状态码
来源：http://hz.jianghu66.top/gtihxclvvt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydzc1.top/gtevocvtmx.html

[R61] 磁盘占用
来源：http://hz.mhx1999.top/gtxwjvpxoj.html

df -h;  du -sh *
来源：http://hz.shangyingyoupin.top/gtdidfgpyh.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gtwcxqlxkt.html

du -ah . | sort -rh | head -10
来源：http://hz.dashuyun.cn/gtkhvroxcm.html

[R63] 内存与进程
来源：http://hz.ywan-chungtsiang.top/gtfuexmvgw.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gtstaloscf.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtzfnuqcul.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtzezjbwyw.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gtjqgluawk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydjk.org.cn/gtqfahcdmj.html

[R66] 定时任务
来源：http://hz.nwbrower.top/gtuzibfkmf.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtfbugyrrz.html

[R67] 生成随机十六进制串
来源：http://hz.haohaochexian.top/gtxzoirlgh.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtfusluakk.html

[R68] 计算文件校验值
来源：http://hz.jiagoushi.top/gtuncgzdix.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dashuyun.cn/gtkkfuuvck.html

[R69] 生成随机密码
来源：http://hz.yueranfly.top/gtybdcvfrc.html

head -c 16 /dev/urandom | base64
来源：http://hz.xinyue.icu/gtirpmeztl.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtcifycvaa.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtscupyfrz.html

[R71] 日期格式化
来源：http://hz.cheryme.top/gtunfsyajd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yanxiufei.cn/gtzcdaontl.html

[R72] 等待端口就绪
来源：http://hz.redwolf501.top/gtqvbjfnhl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtpkqnquxg.html

[R73] 分割大日志
来源：http://hz.mhx1999.top/gtkoztiteq.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtihrubixn.html

[R74] 批量重命名
来源：http://hz.ybcxt.top/gtzeczvkgg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gotoacloud.top/gtwbwvfaqz.html

[R75] 导出环境变量
来源：http://hz.zhixingplan.top/gtbfjdhezu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ppjwa.cn/gtkajexmzf.html

[R76] 使用临时文件
来源：http://hz.xylfe.cn/gtwgsjcrvx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtuwzajfhp.html

[R77] 读取用户输入
来源：http://hz.zhaomingkeji.xyz/gtafwniqgi.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtywpzilru.html

[R78] 交互式菜单
来源：http://hz.yj202588.top/gtdmfbaugb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cqqwz.cn/gtvgwuajvm.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtflzvievw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtsvwrreor.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigfzy.top/gtxweyiaid.html

time ./run.sh
来源：http://hz.hammf.cn/gtakiznnao.html

================================================================================
来源：http://hz.316326.xyz/gthnzlytnl.html

S. C / C++ 专题
来源：http://hz.hammf.cn/gtumqarngm.html

================================================================================
来源：http://hz.c1oappe.top/gtclmlhsca.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtfxnjrtqq.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtzzqzkydj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydzc1.top/gtakgobgxn.html

[S02] C：变量与格式化输出
来源：http://hz.tanke756.top/gtqyqoaqfu.html

int a = 10; printf("%d\n", a);
来源：http://hz.meibo888.top/gtuvhivdti.html

[S03] C：读入整数
来源：http://hz.birdmap.top/gtblhuqqvi.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gtthzfkiqy.html

[S04] C：字符串复制
来源：http://hz.0kj1m.cn/gtngmqnuoc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hywenlv.cn/gtyxuizheg.html

[S05] C：字符串长度
来源：http://hz.aibaodan.cn/gtixjsvtub.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtcinrwhey.html

[S06] C：字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtbtmtnlqc.html

strcmp(a, b) == 0
来源：http://hz.ppjwa.cn/gtjhkalnie.html

[S07] C：数组遍历求和
来源：http://hz.yj20258.top/gtupmkahfa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj20258.top/gtquoehlya.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtzzyjsigh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgfzy.top/gtlnvkdaof.html

[S09] C：结构体定义与初始化
来源：http://hz.52xcode.cn/gtwcycwftv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jianghu66.top/gtfpzyndiv.html

[S10] C：指针与解引用
来源：http://hz.zhaomingkeji.xyz/gtqgpwegkc.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtdzsxfqyn.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gtesmiwdzy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gtepeheyde.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cheryme.top/gtbytqiruw.html

fclose(f);
来源：http://hz.kuanghao11.cn/gtccjlusdm.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtpjkdawso.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hywenlv.cn/gtcmwgfuvp.html

[S13] C：宏定义
来源：http://hz.yj20258888.top/gtiludyqcg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yongpay.top/gtdowenbzz.html

[S14] C：枚举
来源：http://hz.yangfankeji.com/gtqklrugoa.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hysaishi.cn/gtutbibfnz.html

[S15] C：类型转换
来源：http://hz.yj202588.top/gtjofyswph.html

(double) a / b
来源：http://hz.guowangkeji.top/gtwalcuahu.html

[S16] C：位操作置位
来源：http://hz.fzhhl.top/gttggntlza.html

x |= (1 << 3);
来源：http://hz.xingfuxueyuan.xyz/gtiakqmxji.html

[S17] C：安全拼接字符串
来源：http://hz.aizwys.cn/gtxxrluxen.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258.top/gtrzhmmvrm.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtypxmfisb.html

int main(int argc, char **argv)
来源：http://hz.fengsongda.top/gtcyohmidq.html

[S19] C：快速排序
来源：http://hz.fzhhl.top/gtbbqmbcla.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dianchejie.cn/gtlzicopvr.html

[S20] C：二分查找
来源：http://hz.fzhhl.top/gtctpbyqto.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtvcfhehro.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtzjnlnxgx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtxpclfowy.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gthowlptdu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtzprziheb.html

[S23] C：随机数
来源：http://hz.andypj.xyz/gtlgsxoqws.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yanxiufei.cn/gtptimysog.html

[S24] C：获取本地时间
来源：http://hz.hywenlv.cn/gtugbxybvf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.vqdsnc.cn/gtzhylgfqk.html

[S25] C：内存拷贝
来源：http://hz.gogol.net.cn/gtnhsuvyto.html

memcpy(dst, src, n);
来源：http://hz.kuanghao11.cn/gtzreqssmw.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gttxcvgjun.html

memset(a, 0, sizeof a);
来源：http://hz.jiagoushi.top/gtrvxkekgj.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtmoilxqfg.html

const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gtrjukfohk.html

[S28] C：静态变量
来源：http://hz.yuanzhike.top/gtiviaqhti.html

static int counter = 0;
来源：http://hz.dashuyun.cn/gtfpctlobi.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtywbwjmsg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hywenlv.cn/gtaauicqan.html

[S30] C：头文件保护
来源：http://hz.xinyue.icu/gtijwmerts.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gtxuxojejl.html

#define X_H
来源：http://hz.gogol.net.cn/gtjfnjyixs.html

#endif
来源：http://hz.zhixingplan.top/gtczxyiinr.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtytlfzige.html

#include <iostream>
来源：http://hz.andypj.xyz/gtpngjrpow.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cucudq.cn/gtvmbtisgy.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gthmspijce.html

std::string s = "hi";  s += "!";
来源：http://hz.chenzaomai.com/gtwblpjtrl.html

[S33] C++：vector 增删
来源：http://hz.hfpthk.cn/gtuexxtofm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydzc1.top/gtusskmvqh.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gtkmeweoyy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gzhubu.top/gtzjorxbii.html

[S35] C++：map
来源：http://hz.jinqigufen.top/gtqogykhen.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtkypeeepc.html

[S36] C++：unordered_map
来源：http://hz.bjfxy.top/gtvrzdsuyo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtjgpxqbvl.html

[S37] C++：set
来源：http://hz.jianghu66.top/gtezbuggqa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ivvv.top/gtorcwanmx.html

[S38] C++：排序
来源：http://hz.zdqjudy.top/gtoobhrree.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtfzijhkzi.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtgejafxck.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yuxming.cn/gtlrjsjagn.html

[S40] C++：查找元素
来源：http://hz.ybcxt.top/gtstcrpygi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.52xcode.cn/gtvtgwpdle.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtvrrdzrbp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhijiandao.cn/gtydwbtcir.html

[S42] C++：继承与虚函数
来源：http://hz.ppjwa.cn/gtekwbmbvy.html

class B : public Base { public: void f() override {} };
来源：http://hz.zdqjudy.top/gthtcjvdsm.html

[S43] C++：智能指针
来源：http://hz.c1oappe.top/gtmmfppkhw.html

auto p = std::make_unique<int>(5);
来源：http://hz.c1oappe.top/gtwyyvymar.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtngmoslwf.html

void inc(int &x) { ++x; }
来源：http://hz.pycfn.com/gtflfecqoa.html

[S45] C++：lambda
来源：http://hz.sweek.top/gtqvgsjaku.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jianghu66.top/gtkxjucdef.html

[S46] C++：函数模板
来源：http://hz.yj20258.top/gtbgqfkndj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtejbzbgof.html

[S47] C++：结构化绑定遍历
来源：http://hz.feifeiyinyue.top/gtxjdmabfg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ppjwa.cn/gtbhzayrfh.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtgvbigmwq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuxming.cn/gtfxxzgrmm.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtwuobokpo.html

[S49] C++：写文件
来源：http://hz.ehwqpu.com/gtyjzcqull.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.haohaochexian.top/gtktolerjy.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gteaxhsfym.html


<!-- 参考信息 -->