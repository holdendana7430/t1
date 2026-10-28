代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtltkphrix.html

[Q75] 日期格式化
来源：http://hz.meibo888.top/gtzjhjbwil.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ydjk.org.cn/gtfdnvkcfb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jlsjyb.cn/gtljrymhmp.html

[Q76] 按天统计
来源：http://hz.yueranfly.top/gtyglnjkma.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gogol.net.cn/gtabpkprig.html

[Q77] 时间加减
来源：http://hz.meibo888.top/gtzquogkau.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jlsjyb.cn/gtsdbmkwgq.html

[Q78] 当前时间
来源：http://hz.haohaochexian.top/gtgwbvsozj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dianchejie.cn/gthjylpzgc.html

[Q79] 字符串拼接
来源：http://hz.jinqigfzy.top/gtlfannfxi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shangyingyoupin.top/gtswuhuzzu.html

[Q80] 字符串截取
来源：http://hz.guowangkeji.top/gtnjxtbbyy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.redwolf501.top/gtphibanag.html

[Q81] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gttkrlcddz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zycfv.cn/gtllflnyyy.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtykncufzw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.daria6918.cn/gtxbeffdhl.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtppeglxtv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gtiettgggf.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gttpfgygzr.html

SELECT TRIM(name) FROM users;
来源：http://hz.zycfv.cn/gtsvpmogou.html

[Q85] 数值取整
来源：http://hz.bjfxy.top/gtatovwxrv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydzc1.top/gtxskifghl.html

[Q86] 读取 JSON 字段
来源：http://hz.hfpthk.cn/gttdremnbh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.quarkkingdee.top/gtmcpnuhkh.html

[Q87] JSON 字段做条件
来源：http://hz.gotoacloud.top/gtyeljfvhn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cashguo.top/gtkldqcbmm.html

[Q88] 行转列（条件聚合）
来源：http://hz.yuxming.cn/gtvzjstafi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.redwolf501.top/gttgilnbnr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yangfankeji.com/gtydhllvor.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtlsixdees.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinyuanbaomall.cn/gtwgvwzueu.html

[Q90] 生成序号列
来源：http://hz.aibaodan.cn/gtpemwnfwf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xylfe.cn/gttcvxtllf.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtoyxugufp.html

R. Bash 专题
来源：http://hz.hysaishi.cn/gtsgpxlgjf.html

================================================================================
来源：http://hz.cdnleiting.top/gthmpmcoie.html

[R01] shebang 与严格模式
来源：http://hz.zhijiandao.cn/gtnturoyuu.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gtvkxldnbm.html

set -euo pipefail
来源：http://hz.jyoumei.cn/gttjogzoac.html

[R02] 变量赋值与使用
来源：http://hz.ehwqpu.com/gtszbivqiy.html

name="Tom"; echo "$name"
来源：http://hz.xinyue.icu/gtlpgeswhq.html

[R03] 只读变量
来源：http://hz.zhoulong.xyz/gthlgswvyh.html

readonly PI=3.14
来源：http://hz.sysykeji.top/gtbgpoyxed.html

[R04] 位置参数
来源：http://hz.zhongyouzk.top/gtkdgafafn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nwbrower.top/gtjmmtbtzp.html

[R05] 参数默认值
来源：http://hz.hnxiangtu.top/gtyxxnarox.html

name="${1:-default}"
来源：http://hz.svipenyu.cn/gtyrrzebsz.html

[R06] 判断命令是否存在
来源：http://hz.yuanzhike.top/gtutuoayqv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.bjfxy.top/gthyeatttv.html

[R07] if 判断文件
来源：http://hz.0kj1m.cn/gtlcimshbe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tanke756.top/gtplhsfwzn.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gthlyrmhrs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gogol.net.cn/gtaoqthrwx.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtbywkifsh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hywenlv.cn/gtfyvliwwo.html

[R10] 正则匹配
来源：http://hz.tianlin.xyz/gtyyrarplw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gaohongyu789.top/gtrofvgqhp.html

[R11] case 多分支
来源：http://hz.sysykeji.top/gtnmtogcuq.html

case "$1" in
来源：http://hz.zhoulong.xyz/gtywfvzkaj.html

start) echo "启动" ;;
来源：http://hz.chenjidiqi.icu/gtbicphowh.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gtpvqeafaa.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtfmzeydwg.html

esac
来源：http://hz.snrcjt.cn/gtnubduvat.html

[R12] for 遍历文件
来源：http://hz.pycfn.com/gtchaxwdbw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jlsjyb.cn/gtyqundpvo.html

[R13] for 计数循环
来源：http://hz.cucudq.cn/gtesdatcbo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gtpuiqvskk.html

[R14] C 风格 for
来源：http://hz.zhixingplan.top/gtqhkmfmtl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xziqi.cn/gtablmvzjr.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gtemlslnlk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nwbrower.top/gtpxplsipy.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gtiimofmza.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtoeuhhcuk.html

[R17] 数组定义与取值
来源：http://hz.birdmap.top/gtgbpznhnw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.c1oappe.top/gtuyeqkrrm.html

[R18] 遍历数组
来源：http://hz.xylfe.cn/gtrtnnvmbx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtehmadujs.html

[R19] 数组长度
来源：http://hz.tianlin.xyz/gtmaypubhl.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtcsyblizn.html

[R20] 关联数组（字典）
来源：http://hz.bjfxy.top/gteqaehgyt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhongyouzk.top/gtvnvfjsgn.html

[R21] 字符串长度
来源：http://hz.iojbl.cn/gtjzldpxpl.html

echo "${#s}"
来源：http://hz.zdqjudy.top/gtfvzewjzp.html

[R22] 截取子串
来源：http://hz.nanxuanxn.top/gtvgsuklsg.html

echo "${s:0:5}"
来源：http://hz.havefunace.top/gtxwtsabeh.html

[R23] 字符串替换
来源：http://hz.havefunace.top/gtnvugtcuk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj202588.top/gtwepzefex.html

[R24] 大小写转换
来源：http://hz.sweek.top/gtjaldqslh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgfzy.top/gtaxlgcrmt.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgufenzy.top/gtardgjziu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cucudq.cn/gtzptovsxe.html

[R26] 命令替换
来源：http://hz.gogol.net.cn/gtpxnnwoip.html

now=$(date +%F); echo "$now"
来源：http://hz.hongshengwenyu.top/gtkjbbdqrf.html

[R27] 算术展开
来源：http://hz.52xcode.cn/gtmowjwikk.html

echo $((1 + 2 * 3))
来源：http://hz.yongpay.top/gtzycoedpc.html

[R28] 浮点运算
来源：http://hz.svipenyu.cn/gtijxlzplg.html

echo "scale=2; 10/3" | bc
来源：http://hz.yuanzhike.top/gthwygosae.html

[R29] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtklnmxqen.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhongyouzk.top/gthcbyouiw.html

[R30] 函数返回状态码
来源：http://hz.chenjidiqi.icu/gtqztuwjcf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.mhx1999.top/gtskqpspnt.html

[R31] 局部变量
来源：http://hz.shangyingyoupin.top/gtnwnzemnz.html

f() { local x=1; echo "$x"; }
来源：http://hz.guowangkeji.top/gtajmptovz.html

[R32] 参数个数校验
来源：http://hz.jinyuanbaomall.cn/gtjoqjyrmh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cashguo.top/gtljpunjhi.html

[R33] 捕获错误并提示行号
来源：http://hz.meibo888.top/gtyrcqypzn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ivvv.top/gtiiuvzpce.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtizpgswbo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtgumvifgz.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtheudcntw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.snrcjt.cn/gtgmhnjtwa.html

[R36] 并发执行多个任务
来源：http://hz.andypj.xyz/gtfcfatrak.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gaohongyu789.top/gtfbqihmhd.html

[R37] 把输出赋给变量
来源：http://hz.snrcjt.cn/gtuvimmxyo.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtpxqzbezu.html

[R38] 管道串联
来源：http://hz.fengsongda.top/gtwpbxwjus.html

cat a.txt | grep -i error | wc -l
来源：http://hz.redwolf501.top/gtkxmlwajs.html

[R39] 重定向标准输出与错误
来源：http://hz.gogol.net.cn/gtnxgvtxvi.html

cmd > out.log 2>&1
来源：http://hz.chenjidiqi.icu/gtcwgyefgc.html

[R40] 追加写日志
来源：http://hz.birdmap.top/gtrpedyhrx.html

echo "log" >> out.log
来源：http://hz.nwbrower.top/gtzmeralcb.html

[R41] 丢弃输出
来源：http://hz.yuanzhike.top/gtxtfoilpo.html

cmd >/dev/null 2>&1
来源：http://hz.nanxuanxn.top/gtowcwwcjf.html

[R42] 输入重定向
来源：http://hz.jyoumei.cn/gtbdldfqrm.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtkayhgifv.html

[R43] 按名字查找文件
来源：http://hz.shanyushiyangtech.top/gtuzldyxeq.html

find . -name "*.log" -type f
来源：http://hz.wangdashe.top/gtelcobezc.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gtlarzanzd.html

find . -mtime -7 -type f
来源：http://hz.c1oappe.top/gtyvdndpct.html

[R45] 批量删除
来源：http://hz.haohaochexian.top/gtffeuskmg.html

find . -name "*.tmp" -delete
来源：http://hz.hfpthk.cn/gtjzcnnibc.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtzubltfsa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtulxlnwsp.html

[R47] sed 单行替换
来源：http://hz.pengpengdd.cyou/gtgszspgnu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.redwolf501.top/gthqgndkkw.html

[R48] awk 取指定列
来源：http://hz.zhoulong.xyz/gttknbnmgb.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gtjnhzqhhw.html

[R49] awk 带条件
来源：http://hz.havefunace.top/gtdkmvkvmm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shanyushiyangtech.top/gtivwuooox.html

[R50] awk 求和
来源：http://hz.sufxvd.cn/gtzrxxiwip.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shuidangran.top/gtvqjxremh.html

[R51] 排序去重取前几
来源：http://hz.guowangkeji.top/gtnprrwkoo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hywenlv.cn/gtngpnlsig.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtnrlojvxj.html

wc -l a.txt
来源：http://hz.yj20258888.top/gtlqhqlhgv.html

[R53] 查看文件头与实时尾
来源：http://hz.sufxvd.cn/gtzslqvfuy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhaomingkeji.xyz/gtkmqczfre.html

[R54] 比较两个文件
来源：http://hz.shuidangran.top/gtfcbytkxo.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtdzvbljkv.html

[R55] 压缩与解压
来源：http://hz.jiagoushi.top/gtkmgkerna.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.kuanghao11.cn/gtotpxjnbx.html

[R56] 远程拷贝
来源：http://hz.cqqwz.cn/gtloqnnler.html

scp file user@host:/path/
来源：http://hz.jinqigufen.top/gtugcsjumz.html

[R57] 远程执行命令
来源：http://hz.gaohongyu789.top/gtphekcvtw.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gthedupiba.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtxumnjymj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxuanxn.top/gtnlevoccn.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gtgxdyjdkf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gtiiyevthy.html

[R60] 只看 HTTP 状态码
来源：http://hz.xylfe.cn/gtspnooclw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sysykeji.top/gtqixzalow.html

[R61] 磁盘占用
来源：http://hz.mhx1999.top/gtcjzosxnp.html

df -h;  du -sh *
来源：http://hz.yvedp.cn/gthsjqillk.html

[R62] 找最占空间的文件
来源：http://hz.fengsongda.top/gtsngmgwrx.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxinkj.top/gtnataipbx.html

[R63] 内存与进程
来源：http://hz.daxiang520.top/gtzkwxibjm.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtsnzddouk.html

[R64] 结束进程
来源：http://hz.tianlin.xyz/gtltddwiiv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shuidangran.top/gtbdbsvase.html

[R65] 查看端口占用
来源：http://hz.xuetiantiany.cn/gtiegasxyv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtnbzulsub.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gttqteiiek.html

crontab -e;  crontab -l
来源：http://hz.pengpengdd.cyou/gtdxygnnge.html

[R67] 生成随机十六进制串
来源：http://hz.zhijiandao.cn/gtbtyvnrrv.html

openssl rand -hex 16
来源：http://hz.jyoumei.cn/gtsnwscqyv.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtozvbnhfk.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtidhszppp.html

[R69] 生成随机密码
来源：http://hz.zhongyouzk.top/gtydshmplp.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gtuilmyeyw.html

[R70] 时间戳与互转
来源：http://hz.zhixingplan.top/gtdzydsicb.html

date +%s;  date -d @1700000000
来源：http://hz.guowangkeji.top/gtfxosecou.html

[R71] 日期格式化
来源：http://hz.meibo888.top/gttmcxxtvq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.9152youxi.cn/gtzpzvodfw.html

[R72] 等待端口就绪
来源：http://hz.sysykeji.top/gtrppeyequ.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtnvydxrkc.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtpsvwtdre.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtwztwevqb.html

[R74] 批量重命名
来源：http://hz.kuanghao11.cn/gtpopzoaqr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtpnbetkzi.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtcwyqyoop.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtpsjyyrrt.html

[R76] 使用临时文件
来源：http://hz.jqgufenzy.top/gtqpupossc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtlqxtrdnh.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtfpumsyuj.html

read -rp "请输入: " ans
来源：http://hz.zhiwuduotai.top/gtzrkyyckm.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtizzwirhe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.redwolf501.top/gtnqqjypat.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtpvdnxcqh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gthceftilr.html

[R80] 查看脚本执行耗时
来源：http://hz.jiagoushi.top/gtasrwlcda.html

time ./run.sh
来源：http://hz.smart0.xyz/gtwrxfgfyp.html

================================================================================
来源：http://hz.tian-w.cn/gtvvykxtbs.html

S. C / C++ 专题
来源：http://hz.zdqjudy.top/gtimlbilha.html

================================================================================
来源：http://hz.hysaishi.cn/gtzfisvciq.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtaqrdennh.html

#include <stdio.h>
来源：http://hz.yangfankeji.com/gtkusevkul.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.aibaodan.cn/gtozylqhdx.html

[S02] C：变量与格式化输出
来源：http://hz.iojbl.cn/gthbudviov.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnqzz.top/gtxphosftq.html

[S03] C：读入整数
来源：http://hz.chenzaomai.com/gtmuvpqlyo.html

int x; scanf("%d", &x);
来源：http://hz.hongshengwenyu.top/gtptxthmfu.html

[S04] C：字符串复制
来源：http://hz.jyoumei.cn/gtktukwpad.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cheryme.top/gtxmbtdckn.html

[S05] C：字符串长度
来源：http://hz.kuanghao11.cn/gtsqeukskl.html

strlen(s)
来源：http://hz.ivvv.top/gtiogkqiti.html

[S06] C：字符串比较
来源：http://hz.ydzc1.top/gtojrddxkk.html

strcmp(a, b) == 0
来源：http://hz.pycfn.com/gtwbnzmfeu.html

[S07] C：数组遍历求和
来源：http://hz.zhaomingkeji.xyz/gtwnoylyll.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sweek.top/gtlyjxsyqg.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgufenzy.top/gtygdwifew.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gzhubu.top/gtfixhludq.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gtxpyanwvk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnxiangtu.top/gtikerdvas.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangkeji.top/gtgoxfnwrd.html

int *p = &a;  *p = 5;
来源：http://hz.shzxlz.cn/gtgdanxyrr.html

[S11] C：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtdmmeifnc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sweek.top/gtrblnpsnv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gtzcuzwapa.html

fclose(f);
来源：http://hz.gogol.net.cn/gtikaqjpct.html

[S12] C：写文件
来源：http://hz.0kj1m.cn/gthelkmzty.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hfpthk.cn/gtjlbqgwml.html

[S13] C：宏定义
来源：http://hz.yuxming.cn/gtmohnxnsv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.mhx1999.top/gthtcqxwue.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtkidhjoco.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ehwqpu.com/gtkvixdytr.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gtobgkkauw.html

(double) a / b
来源：http://hz.cashguo.top/gttzfiubvu.html

[S16] C：位操作置位
来源：http://hz.smart0.xyz/gtlpnovzuv.html

x |= (1 << 3);
来源：http://hz.ppjwa.cn/gtkosmecdq.html

[S17] C：安全拼接字符串
来源：http://hz.hywenlv.cn/gtbwokssts.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtqsohmaeg.html

[S18] C：命令行参数
来源：http://hz.sxryk.cn/gtagyfkapq.html

int main(int argc, char **argv)
来源：http://hz.yuxming.cn/gtzzjvfmlt.html

[S19] C：快速排序
来源：http://hz.52xcode.cn/gtslpdkafo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtwbahiooz.html

[S20] C：二分查找
来源：http://hz.sysykeji.top/gtouoeqrwu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtcpzjxdor.html

[S21] C：字符类别判断
来源：http://hz.nanxuanxn.top/gtcznfyads.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gteciyqjaw.html

[S22] C：字符串转数字
来源：http://hz.0kj1m.cn/gtbbptfjbg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jlsjyb.cn/gtqdmilnef.html

[S23] C：随机数
来源：http://hz.jyoumei.cn/gtmmhnwiop.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cucudq.cn/gtdaajtwye.html

[S24] C：获取本地时间
来源：http://hz.jlsjyb.cn/gtoetbfdan.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gtlqpmrfpd.html

[S25] C：内存拷贝
来源：http://hz.gotoacloud.top/gtcdwgjwur.html

memcpy(dst, src, n);
来源：http://hz.sxryk.cn/gtfdqwwdia.html

[S26] C：内存清零
来源：http://hz.xuanzx.com/gtpkejsbtt.html

memset(a, 0, sizeof a);
来源：http://hz.guannengcc.top/gthudydpxt.html

[S27] C：定义常量
来源：http://hz.kuanghao11.cn/gthcqfyaxe.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtjhylqqej.html

[S28] C：静态变量
来源：http://hz.dashuyun.cn/gtjnupzlmp.html

static int counter = 0;
来源：http://hz.xylfe.cn/gthzwiqaxn.html

[S29] C：变参函数
来源：http://hz.wangshuangyany.cn/gthigcwgtz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pycfn.com/gtsqdbwcji.html

[S30] C：头文件保护
来源：http://hz.zhongyouzk.top/gtfxfmngjz.html

#ifndef X_H
来源：http://hz.xylfe.cn/gtyifwdzjn.html

#define X_H
来源：http://hz.zhijiandao.cn/gtphaxzhxx.html

#endif
来源：http://hz.zhoulong.xyz/gtdygltzgi.html

[S31] C++：Hello World
来源：http://hz.zhijiandao.cn/gtriamkfhn.html

#include <iostream>
来源：http://hz.haohaochexian.top/gtumcddffz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hysaishi.cn/gtsrtehqbe.html

[S32] C++：字符串
来源：http://hz.jinyuanbaomall.cn/gtjmxzbzsa.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtmsuejoxt.html

[S33] C++：vector 增删
来源：http://hz.zhiwuduotai.top/gtrpewisyd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtdmrgzaxt.html

[S34] C++：遍历 vector
来源：http://hz.mhx1999.top/gtyrwzrbpv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shangyingyoupin.top/gtzyevxdbx.html

[S35] C++：map
来源：http://hz.cashguo.top/gtexsieweh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hongshengwenyu.top/gtxscnpkym.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtimawdrma.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtpkmerwaa.html

[S37] C++：set
来源：http://hz.gotoacloud.top/gtpkkrxcak.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shuidangran.top/gtsdptfxot.html

[S38] C++：排序
来源：http://hz.jqgfzy.top/gtebyvkdwz.html

std::sort(v.begin(), v.end());
来源：http://hz.c1oappe.top/gtyyjrxcrm.html

[S39] C++：自定义比较器排序
来源：http://hz.xingfuxueyuan.xyz/gtohnfvglg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xingfuxueyuan.xyz/gtjqgxrugm.html

[S40] C++：查找元素
来源：http://hz.gzhubu.top/gtmzynrytt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtgpagwiir.html

[S41] C++：类与构造函数
来源：http://hz.gzhubu.top/gtsjkrxnxq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gtfxbbxzfv.html

[S42] C++：继承与虚函数
来源：http://hz.chenlongwang.top/gtjftsqnmo.html

class B : public Base { public: void f() override {} };
来源：http://hz.shuidangran.top/gtsotwsntd.html

[S43] C++：智能指针
来源：http://hz.pycfn.com/gtsrxpofzz.html

auto p = std::make_unique<int>(5);
来源：http://hz.iojbl.cn/gtaiiitfxi.html

[S44] C++：引用传参
来源：http://hz.ybcxt.top/gtjsaunmqd.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtvvjuodhz.html


<!-- 参考信息 -->