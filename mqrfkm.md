代发 wailian999

[Q80] 字符串截取
来源：http://hz.tian-w.cn/gtwaqrtwen.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.smart0.xyz/gtakwitpcr.html

[Q81] 字符串替换
来源：http://hz.redwolf501.top/gtsnfstofv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.aizwys.cn/gtkeofntcu.html

[Q82] 字符长度与字节长度
来源：http://hz.kuanghao11.cn/gtrbgzseme.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtadadrxqa.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtegttxsgr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xylfe.cn/gtkmrmentv.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gtfpqyqygp.html

SELECT TRIM(name) FROM users;
来源：http://hz.snrcjt.cn/gthesgjyza.html

[Q85] 数值取整
来源：http://hz.zdqjudy.top/gtwjnjegqo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgfzy.top/gtydycsrqy.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtyzpbnqpy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.vqdsnc.cn/gtubacfvab.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gtgmylbdtd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.haohaochexian.top/gthhivzrac.html

[Q88] 行转列（条件聚合）
来源：http://hz.xingfuxueyuan.xyz/gtgdjikjxl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtpapyxmhm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yueranfly.top/gtxpcnvvrr.html

[Q89] 判断表是否存在
来源：http://hz.shangyingyoupin.top/gtyfyhmybu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xingfuxueyuan.xyz/gtbbrezbdn.html

[Q90] 生成序号列
来源：http://hz.ydjk.org.cn/gtuofrynqh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aibaodan.cn/gtzmobtxjt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqmzdiaxa.html

R. Bash 专题
来源：http://hz.meibo888.top/gtkgwfhhhb.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtlwqgkdol.html

[R01] shebang 与严格模式
来源：http://hz.daxiang520.top/gtvsznesvs.html

#!/usr/bin/env bash
来源：http://hz.yangfankeji.com/gteegwqedd.html

set -euo pipefail
来源：http://hz.yj20258888.top/gtejlxbsnn.html

[R02] 变量赋值与使用
来源：http://hz.gzhubu.top/gthuphqpcu.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gthmatibky.html

[R03] 只读变量
来源：http://hz.yuanzhike.top/gtshsfjzcz.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtgbodbuvd.html

[R04] 位置参数
来源：http://hz.zhixingplan.top/gtqkmnntqx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.chenjidiqi.icu/gtbmaebsqf.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtrztownlc.html

name="${1:-default}"
来源：http://hz.nwbrower.top/gtiyvpvekw.html

[R06] 判断命令是否存在
来源：http://hz.jqgfzy.top/gtjsrvwaco.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pycfn.com/gtdelaiewv.html

[R07] if 判断文件
来源：http://hz.jinqigufen.top/gtlsgigzxd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtvbuhquij.html

[R08] 数值比较
来源：http://hz.quarkkingdee.top/gtjicdfcli.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhongyouzk.top/gtgqyjfddj.html

[R09] 字符串比较
来源：http://hz.yueranfly.top/gtfqnwdffj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ywan-chungtsiang.top/gtinhxngyl.html

[R10] 正则匹配
来源：http://hz.sweek.top/gtwohnxskf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtjyqcvcso.html

[R11] case 多分支
来源：http://hz.quarkkingdee.top/gtbsrglaua.html

case "$1" in
来源：http://hz.gzhubu.top/gtytznkbgr.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtxzdljaie.html

stop)  echo "停止" ;;
来源：http://hz.kuanghao11.cn/gtcfwdbmpi.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gterrshzww.html

esac
来源：http://hz.iojbl.cn/gtxytkdudb.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtncrpyppv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.birdmap.top/gtddxcdtff.html

[R13] for 计数循环
来源：http://hz.sysykeji.top/gtogxpctma.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtwpavleud.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gtamczxifm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258.top/gtglqzgoon.html

[R15] while 逐行读文件
来源：http://hz.chenzaomai.com/gtmvtotegd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xziqi.cn/gtcjugzhzw.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtpmtprxnn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.mhx1999.top/gtdpmbdzqc.html

[R17] 数组定义与取值
来源：http://hz.daria6918.cn/gtpnswlhjr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtjxrllkwh.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gturvazcnu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhongyouzk.top/gtqgcujamk.html

[R19] 数组长度
来源：http://hz.zycfv.cn/gtlenqvdkh.html

echo "${#arr[@]}"
来源：http://hz.pengpengdd.cyou/gtdgpgkfbo.html

[R20] 关联数组（字典）
来源：http://hz.chenzaomai.com/gtrhuoqhzj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhixingplan.top/gtbtnbkxjm.html

[R21] 字符串长度
来源：http://hz.sweek.top/gtdrfbpfxb.html

echo "${#s}"
来源：http://hz.fzhhl.top/gtvxzmhjtq.html

[R22] 截取子串
来源：http://hz.cdnleiting.top/gtmauusgnu.html

echo "${s:0:5}"
来源：http://hz.jinghuilouyu.cn/gtzaifnurt.html

[R23] 字符串替换
来源：http://hz.chenjidiqi.icu/gtvjpxdems.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.9152youxi.cn/gtxnwbyuhb.html

[R24] 大小写转换
来源：http://hz.sweek.top/gtrrkhcrfg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgfzy.top/gtgsjxnhlm.html

[R25] 去后缀 / 去前缀
来源：http://hz.316326.xyz/gtulahlnrj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gtjaablfab.html

[R26] 命令替换
来源：http://hz.ppjwa.cn/gtmegsekqg.html

now=$(date +%F); echo "$now"
来源：http://hz.yuanzhike.top/gtyffwjosp.html

[R27] 算术展开
来源：http://hz.yonumen.top/gthdhdikwj.html

echo $((1 + 2 * 3))
来源：http://hz.wangshuangyany.cn/gthtraddef.html

[R28] 浮点运算
来源：http://hz.vqdsnc.cn/gtzrnmxlvi.html

echo "scale=2; 10/3" | bc
来源：http://hz.sweek.top/gtdtlvhkpf.html

[R29] 定义函数
来源：http://hz.dashuyun.cn/gterqcugtu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnxiangtu.top/gtqhgfqfjt.html

[R30] 函数返回状态码
来源：http://hz.dianchejie.cn/gtlheinfzh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtrjqrmsha.html

[R31] 局部变量
来源：http://hz.svipenyu.cn/gtotxwgqrr.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtbcvjmjid.html

[R32] 参数个数校验
来源：http://hz.pycfn.com/gtbfozkizi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gthhnbvmck.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gtkbekcare.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.svipenyu.cn/gtqodfxhkq.html

[R34] 退出时清理
来源：http://hz.dashuyun.cn/gtckdhlizn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gttrmlcgnj.html

[R35] 后台执行并等待
来源：http://hz.chenjidiqi.icu/gtwzousyme.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtokmrladg.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtnteojzui.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnqzz.top/gtehbngqls.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtlyudyuen.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtywfbvvgq.html

[R38] 管道串联
来源：http://hz.jqgfzy.top/gtbvawtwys.html

cat a.txt | grep -i error | wc -l
来源：http://hz.svipenyu.cn/gtuhcvqqyi.html

[R39] 重定向标准输出与错误
来源：http://hz.yuxming.cn/gtdomochjs.html

cmd > out.log 2>&1
来源：http://hz.xinyue.icu/gtagqtwbpz.html

[R40] 追加写日志
来源：http://hz.jianghu66.top/gtygobobgi.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtborttgzz.html

[R41] 丢弃输出
来源：http://hz.jinqigfzy.top/gtlcagtqdd.html

cmd >/dev/null 2>&1
来源：http://hz.cucudq.cn/gtcwzmnnhu.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtlvzbanph.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtetopmvxu.html

[R43] 按名字查找文件
来源：http://hz.zhongyouzk.top/gthtplktyb.html

find . -name "*.log" -type f
来源：http://hz.quarkkingdee.top/gtdsowzguy.html

[R44] 按修改时间查找
来源：http://hz.smart0.xyz/gteaysynsv.html

find . -mtime -7 -type f
来源：http://hz.kuanghao11.cn/gtswxgworh.html

[R45] 批量删除
来源：http://hz.0kj1m.cn/gtgvakrxkj.html

find . -name "*.tmp" -delete
来源：http://hz.zycfv.cn/gtmogdydut.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtvktbrgvu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xziqi.cn/gtwzbganug.html

[R47] sed 单行替换
来源：http://hz.52xcode.cn/gtdrfxtrko.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jqgfzy.top/gtjliurukh.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gtnswkeihn.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtcsnpbwmq.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtiybktgcq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtogkwrmod.html

[R50] awk 求和
来源：http://hz.hfpthk.cn/gtzximgmwf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtusbxgefw.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtmrxlekhs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.fengsongda.top/gtywzxdvmy.html

[R52] 统计行数
来源：http://hz.ppjwa.cn/gthzdndpqy.html

wc -l a.txt
来源：http://hz.hnxiangtu.top/gtdojmnrhk.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtneogxvdj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtxgbyrkbt.html

[R54] 比较两个文件
来源：http://hz.sufxvd.cn/gtckjvumkx.html

diff a.txt b.txt
来源：http://hz.shanyushiyangtech.top/gtpvggfclf.html

[R55] 压缩与解压
来源：http://hz.wangshuangyany.cn/gtdolwgjev.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gtfbcvhedb.html

[R56] 远程拷贝
来源：http://hz.jinqigufen.top/gtmaqcglxm.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gttaqeosty.html

[R57] 远程执行命令
来源：http://hz.sxryk.cn/gtxwmgxgkf.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtzsnawajw.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtqyjsrbjv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuanzhike.top/gtsmjyzcos.html

[R59] 发 POST JSON
来源：http://hz.cucudq.cn/gtlopecuvf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.birdmap.top/gtcijociwj.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtvaryghbu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtfzclnsnd.html

[R61] 磁盘占用
来源：http://hz.ydjk.org.cn/gtlaiyyzcv.html

df -h;  du -sh *
来源：http://hz.ppjwa.cn/gtfrkbprer.html

[R62] 找最占空间的文件
来源：http://hz.zhongyouzk.top/gtlwvkjlyc.html

du -ah . | sort -rh | head -10
来源：http://hz.jlsjyb.cn/gtudksfmqf.html

[R63] 内存与进程
来源：http://hz.sxryk.cn/gtedjytong.html

free -h;  ps aux | grep nginx
来源：http://hz.daria6918.cn/gtexxdjgmk.html

[R64] 结束进程
来源：http://hz.iojbl.cn/gtemtivwsy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258888.top/gttqieeycl.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtonpppiuu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.316326.xyz/gtqdkvauog.html

[R66] 定时任务
来源：http://hz.svipenyu.cn/gtxonaxwts.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gtcddbupcb.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtptfhbfbm.html

openssl rand -hex 16
来源：http://hz.xylfe.cn/gtoukvxcjf.html

[R68] 计算文件校验值
来源：http://hz.cqqwz.cn/gtncizryhg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnxiangtu.top/gtnahyuslh.html

[R69] 生成随机密码
来源：http://hz.ehwqpu.com/gtjvlyanlr.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuanzhike.top/gtinconfes.html

[R70] 时间戳与互转
来源：http://hz.redwolf501.top/gtlwicfxrq.html

date +%s;  date -d @1700000000
来源：http://hz.fengsongda.top/gtuqvxufyk.html

[R71] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gttdsfgfyf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.vqdsnc.cn/gtpargcrzg.html

[R72] 等待端口就绪
来源：http://hz.fzhhl.top/gtrflflgqd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtepkihabl.html

[R73] 分割大日志
来源：http://hz.sysykeji.top/gtiexehkci.html

split -l 1000 big.log part_
来源：http://hz.xuanzx.com/gtmevirytr.html

[R74] 批量重命名
来源：http://hz.guowangkeji.top/gtmrpfwxef.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yvedp.cn/gtlcukccna.html

[R75] 导出环境变量
来源：http://hz.tianlin.xyz/gtlexmawwm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtonzatdyj.html

[R76] 使用临时文件
来源：http://hz.xingfuxueyuan.xyz/gtrmehdrkx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtvoaozqzd.html

[R77] 读取用户输入
来源：http://hz.quarkkingdee.top/gtecwjduqd.html

read -rp "请输入: " ans
来源：http://hz.yueranfly.top/gtbyzgpptw.html

[R78] 交互式菜单
来源：http://hz.andypj.xyz/gtanxjcnwg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtcknfpilm.html

[R79] 解析命令行选项
来源：http://hz.wangshuangyany.cn/gtvtabyoiv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gogol.net.cn/gtqxgmvvyv.html

[R80] 查看脚本执行耗时
来源：http://hz.kuanghao11.cn/gtnckujhze.html

time ./run.sh
来源：http://hz.sysykeji.top/gtzuqfgiqu.html

================================================================================
来源：http://hz.hfpthk.cn/gtpilvizgd.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gtjqvfbube.html

================================================================================
来源：http://hz.chenzaomai.com/gteurkhtba.html

[S01] C：Hello World
来源：http://hz.ydzc1.top/gtztuiphoh.html

#include <stdio.h>
来源：http://hz.yj202588.top/gtykcqqtpj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtrvhnfrfj.html

[S02] C：变量与格式化输出
来源：http://hz.shzxlz.cn/gtrcfssioz.html

int a = 10; printf("%d\n", a);
来源：http://hz.gzhubu.top/gtouitpgtg.html

[S03] C：读入整数
来源：http://hz.aizwys.cn/gtacwblhhl.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gtbqjpwiqh.html

[S04] C：字符串复制
来源：http://hz.hammf.cn/gttzagicsa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhijiandao.cn/gtmfeijkit.html

[S05] C：字符串长度
来源：http://hz.nanxuanxn.top/gtksyjlltm.html

strlen(s)
来源：http://hz.fengsongda.top/gtnmzstuff.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtsrgbfurk.html

strcmp(a, b) == 0
来源：http://hz.cucudq.cn/gteydbizqm.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtnvsfftxw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ivvv.top/gtgfqbxbij.html

[S08] C：动态内存分配与释放
来源：http://hz.dianchejie.cn/gtlekfxajn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenjidiqi.icu/gtotxqewap.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtuxqtapqu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gotoacloud.top/gteljrdqkl.html

[S10] C：指针与解引用
来源：http://hz.fengsongda.top/gtzuuxpnuh.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtfwxocplj.html

[S11] C：逐行读文件
来源：http://hz.nanxuanxn.top/gtjmzchnui.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gttutuvmgu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gtqffwzhqa.html

fclose(f);
来源：http://hz.meibo888.top/gtewwijcdb.html

[S12] C：写文件
来源：http://hz.yueranfly.top/gtusvgdspr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxinkj.top/gtcclkbhbg.html

[S13] C：宏定义
来源：http://hz.ybcxt.top/gtlwzovgyk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtfvkinslj.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gtdiciroqy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sxryk.cn/gtweelphto.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gtyegsdsba.html

(double) a / b
来源：http://hz.wangdashe.top/gtkawvlzew.html

[S16] C：位操作置位
来源：http://hz.kuanghao11.cn/gtzcxmwdgl.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtrycrgnoy.html

[S17] C：安全拼接字符串
来源：http://hz.dashuyun.cn/gtjauvcght.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinghuilouyu.cn/gtsanwxuph.html

[S18] C：命令行参数
来源：http://hz.kuanghao11.cn/gtruatxbih.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtdhkywlcm.html

[S19] C：快速排序
来源：http://hz.c1oappe.top/gtysfxkfxl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtnvqgihrz.html

[S20] C：二分查找
来源：http://hz.vqdsnc.cn/gtvqlzxvgf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.dianchejie.cn/gtvmswuxug.html

[S21] C：字符类别判断
来源：http://hz.zhoulong.xyz/gtpivtcbeu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xingfuxueyuan.xyz/gtzeelzkgr.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gtgzogujji.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yvedp.cn/gtepejysws.html

[S23] C：随机数
来源：http://hz.tanke756.top/gtzgtajehg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhoulong.xyz/gtfdeajlsn.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtxvbwafjh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258.top/gtyctpyktx.html

[S25] C：内存拷贝
来源：http://hz.jinqigfzy.top/gtksqlihwv.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtfayguyqg.html

[S26] C：内存清零
来源：http://hz.xziqi.cn/gtecbrinpo.html

memset(a, 0, sizeof a);
来源：http://hz.c1oappe.top/gtxmeibktb.html

[S27] C：定义常量
来源：http://hz.cqqwz.cn/gtblmccwwx.html

const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtonplegki.html

[S28] C：静态变量
来源：http://hz.ppjwa.cn/gtimhomgwx.html

static int counter = 0;
来源：http://hz.guowangkeji.top/gtzxmceqof.html

[S29] C：变参函数
来源：http://hz.zycfv.cn/gtsdcliqnb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fengsongda.top/gtlsujxocc.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtlijyvehb.html

#ifndef X_H
来源：http://hz.tianlin.xyz/gtvcgauqmc.html

#define X_H
来源：http://hz.jiagoushi.top/gtoernjaaz.html

#endif
来源：http://hz.yj20258.top/gtesanlnsw.html

[S31] C++：Hello World
来源：http://hz.cashguo.top/gtspxtcdnn.html

#include <iostream>
来源：http://hz.jinyuanbaomall.cn/gtvhcldxgo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.havefunace.top/gtrtteqqwf.html

[S32] C++：字符串
来源：http://hz.hysaishi.cn/gtkgliewnp.html

std::string s = "hi";  s += "!";
来源：http://hz.meibo888.top/gtbjemqyag.html

[S33] C++：vector 增删
来源：http://hz.nanxuanxn.top/gtrniywufi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.andypj.xyz/gtlegtlfps.html

[S34] C++：遍历 vector
来源：http://hz.meibo888.top/gtdmrrmrst.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yongpay.top/gtmmtwjfbv.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtwhwlofau.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gteccbmijk.html

[S36] C++：unordered_map
来源：http://hz.gaohongyu789.top/gtmnifxktl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtgkvgcvgo.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtffpthffy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtlwogcpes.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gtumrmaucd.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gtiydwfmry.html

[S39] C++：自定义比较器排序
来源：http://hz.snrcjt.cn/gtglibrhbr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gtzifaekyh.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtbxghlhil.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gtygqfarjk.html

[S41] C++：类与构造函数
来源：http://hz.nanxinkj.top/gtqvfxnhsc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guannengcc.top/gtzblwpywl.html

[S42] C++：继承与虚函数
来源：http://hz.sweek.top/gtmsiqnnwv.html

class B : public Base { public: void f() override {} };
来源：http://hz.aibaodan.cn/gtkddjgbjk.html

[S43] C++：智能指针
来源：http://hz.dashuyun.cn/gtuhalgdlh.html

auto p = std::make_unique<int>(5);
来源：http://hz.ppjwa.cn/gthvmuhenw.html

[S44] C++：引用传参
来源：http://hz.hywenlv.cn/gtcechwtgk.html

void inc(int &x) { ++x; }
来源：http://hz.sweek.top/gtfnsndmoc.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gthkahrljw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.redwolf501.top/gtegnozgfg.html

[S46] C++：函数模板
来源：http://hz.pycfn.com/gtklmcwjwv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtvvydzsid.html

[S47] C++：结构化绑定遍历
来源：http://hz.ppjwa.cn/gtkuqvfxoo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.mhx1999.top/gtsilboogj.html

[S48] C++：逐行读文件
来源：http://hz.dianchejie.cn/gtbhtcvtdy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cucudq.cn/gtkcqsqkyb.html

while (std::getline(in, line)) { }
来源：http://hz.guowangkeji.top/gtmafnloja.html

[S49] C++：写文件
来源：http://hz.ydzc1.top/gtuyraxrch.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gtxyqhotsl.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtoisdmgqd.html


<!-- 参考信息 -->