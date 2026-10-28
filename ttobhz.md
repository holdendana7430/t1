代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.shzxlz.cn/gtlpwudwjv.html

[Q73] 查看表状态
来源：http://hz.xziqi.cn/gtwsdvyvaj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtlbkjlhve.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtlaceccdf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.52xcode.cn/gtolowfsqw.html

[Q75] 日期格式化
来源：http://hz.fzhhl.top/gtgzapwqzy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtbsoqzdab.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dashuyun.cn/gtrecgrjjw.html

[Q76] 按天统计
来源：http://hz.meibo888.top/gtghlupffc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtgpydhssn.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtawebemkf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinghuilouyu.cn/gtdxnnxpxw.html

[Q78] 当前时间
来源：http://hz.zdqjudy.top/gtrglmmcga.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tian-w.cn/gtjsdsfjms.html

[Q79] 字符串拼接
来源：http://hz.andypj.xyz/gtcdmxgvqy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.svipenyu.cn/gtrtmfadbi.html

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gtumnlovsk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gotoacloud.top/gtlnmwtyzr.html

[Q81] 字符串替换
来源：http://hz.birdmap.top/gtmffuqeyo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.0kj1m.cn/gtuglsybfb.html

[Q82] 字符长度与字节长度
来源：http://hz.jyoumei.cn/gtyuszueky.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tanke756.top/gtyllnshop.html

[Q83] 大小写转换
来源：http://hz.pycfn.com/gtcowetzpk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtyyxgmbcz.html

[Q84] 去除首尾空格
来源：http://hz.ywan-chungtsiang.top/gtgxpvndwi.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258.top/gtqdrtkpzg.html

[Q85] 数值取整
来源：http://hz.feifeiyinyue.top/gtdmiyozvi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ppjwa.cn/gtfuvmocaz.html

[Q86] 读取 JSON 字段
来源：http://hz.xuanzx.com/gtrbfwxeyq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj202588.top/gtlpzezbyn.html

[Q87] JSON 字段做条件
来源：http://hz.xingfuxueyuan.xyz/gtwmfucvlb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jianghu66.top/gtrxjeszii.html

[Q88] 行转列（条件聚合）
来源：http://hz.shzxlz.cn/gtwkugilvc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gthlnjnhbg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yonumen.top/gtwkenpqxt.html

[Q89] 判断表是否存在
来源：http://hz.wangshuangyany.cn/gtdjdxcrhr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxinkj.top/gtfcmzepmo.html

[Q90] 生成序号列
来源：http://hz.fzhhl.top/gtcjdcivzr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jyoumei.cn/gtizyibbrx.html

================================================================================
来源：http://hz.iojbl.cn/gtidubrupn.html

R. Bash 专题
来源：http://hz.yj20258.top/gtfuuugntm.html

================================================================================
来源：http://hz.ydzc1.top/gtmiipisli.html

[R01] shebang 与严格模式
来源：http://hz.yj202588.top/gtcjssfdec.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gtyellgacb.html

set -euo pipefail
来源：http://hz.dashuyun.cn/gtcvuwditc.html

[R02] 变量赋值与使用
来源：http://hz.chenzaomai.com/gtadkexkhz.html

name="Tom"; echo "$name"
来源：http://hz.ywan-chungtsiang.top/gtoqgqvtce.html

[R03] 只读变量
来源：http://hz.yangfankeji.com/gtmoxfbxhb.html

readonly PI=3.14
来源：http://hz.nanxinkj.top/gthaytllsc.html

[R04] 位置参数
来源：http://hz.shanyushiyangtech.top/gtmwghaubx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.daria6918.cn/gtvfmqaoqw.html

[R05] 参数默认值
来源：http://hz.zhixingplan.top/gtjpwegdug.html

name="${1:-default}"
来源：http://hz.tanke756.top/gtcunljquo.html

[R06] 判断命令是否存在
来源：http://hz.zhoulong.xyz/gtynycqvtc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yuxming.cn/gtopsdbhff.html

[R07] if 判断文件
来源：http://hz.jqgfzy.top/gtbcrebtjd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cqqwz.cn/gtkaffklwj.html

[R08] 数值比较
来源：http://hz.xuanzx.com/gtelytlwjw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cdnleiting.top/gtquulsmkp.html

[R09] 字符串比较
来源：http://hz.zhaomingkeji.xyz/gtcbjvtkhn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtetyyesfj.html

[R10] 正则匹配
来源：http://hz.zycfv.cn/gtknkfrerr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gtxynzzrao.html

[R11] case 多分支
来源：http://hz.yj20258.top/gtlxigqlby.html

case "$1" in
来源：http://hz.snrcjt.cn/gttdzhtqav.html

start) echo "启动" ;;
来源：http://hz.shangyingyoupin.top/gtjxzpjoef.html

stop)  echo "停止" ;;
来源：http://hz.xziqi.cn/gtnkwrjbjc.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtwgaodzlx.html

esac
来源：http://hz.shuidangran.top/gtnzmfasvf.html

[R12] for 遍历文件
来源：http://hz.hysaishi.cn/gtxyrzmszo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gticrhhhtk.html

[R13] for 计数循环
来源：http://hz.ydjk.org.cn/gtnvqdhkvt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtnsjhllrr.html

[R14] C 风格 for
来源：http://hz.guannengcc.top/gtypqggtwy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gzhubu.top/gtxyzfesud.html

[R15] while 逐行读文件
来源：http://hz.sufxvd.cn/gtjclrzvym.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtqagjuurz.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtguwfyzvs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ybcxt.top/gtfjomxovf.html

[R17] 数组定义与取值
来源：http://hz.gzhubu.top/gtroxcanmr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sxryk.cn/gtvxqnxbxw.html

[R18] 遍历数组
来源：http://hz.shzxlz.cn/gtqvkoqkvd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtuivyidbu.html

[R19] 数组长度
来源：http://hz.xziqi.cn/gtdwgszage.html

echo "${#arr[@]}"
来源：http://hz.jqgufenzy.top/gttotuqqam.html

[R20] 关联数组（字典）
来源：http://hz.hnqzz.top/gtkntuycea.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xuetiantiany.cn/gthvowmamb.html

[R21] 字符串长度
来源：http://hz.jinqigufen.top/gttrkgxpin.html

echo "${#s}"
来源：http://hz.birdmap.top/gthdeydsiq.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtvbflvahs.html

echo "${s:0:5}"
来源：http://hz.dashuyun.cn/gtguketrga.html

[R23] 字符串替换
来源：http://hz.snrcjt.cn/gteszgbisv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnxiangtu.top/gtjwdquiud.html

[R24] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtctuytnxm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.smart0.xyz/gtuffgjofs.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtgeoilbmy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nanxinkj.top/gtdiwisjhz.html

[R26] 命令替换
来源：http://hz.shuidangran.top/gtvjoznhgj.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258.top/gtyoisokyx.html

[R27] 算术展开
来源：http://hz.hammf.cn/gtbjdwsous.html

echo $((1 + 2 * 3))
来源：http://hz.tian-w.cn/gtdcpkymif.html

[R28] 浮点运算
来源：http://hz.zycfv.cn/gtunktvcga.html

echo "scale=2; 10/3" | bc
来源：http://hz.sufxvd.cn/gtnuopjaby.html

[R29] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtnoinuwwe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gzhubu.top/gtuskmovdw.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtvaqqgmkj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shuidangran.top/gtadsmdcxt.html

[R31] 局部变量
来源：http://hz.aibaodan.cn/gtlnvvqzrt.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtdacthyvi.html

[R32] 参数个数校验
来源：http://hz.gaohongyu789.top/gtjjgmaicw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtdcsxyqhf.html

[R33] 捕获错误并提示行号
来源：http://hz.shuidangran.top/gtbfehpdxy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.svipenyu.cn/gtnnqlnlnu.html

[R34] 退出时清理
来源：http://hz.yvedp.cn/gtkqcqedlw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtqzqgjqos.html

[R35] 后台执行并等待
来源：http://hz.kuanghao11.cn/gtzyibpeib.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jianghu66.top/gtgbczlzhh.html

[R36] 并发执行多个任务
来源：http://hz.tanke756.top/gtgekqnocd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.meibo888.top/gtrdwdkdip.html

[R37] 把输出赋给变量
来源：http://hz.tanke756.top/gtgorvukky.html

files=$(ls -1)
来源：http://hz.xinyue.icu/gtlyrzkvmz.html

[R38] 管道串联
来源：http://hz.xuanzx.com/gtqmbklnye.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ybcxt.top/gtvgtvqwag.html

[R39] 重定向标准输出与错误
来源：http://hz.yuanzhike.top/gtugvzjrur.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtbqnybjwd.html

[R40] 追加写日志
来源：http://hz.ivvv.top/gtrffdpraf.html

echo "log" >> out.log
来源：http://hz.gotoacloud.top/gthvyplpon.html

[R41] 丢弃输出
来源：http://hz.jqgufenzy.top/gthbqidutd.html

cmd >/dev/null 2>&1
来源：http://hz.xuanzx.com/gtvashkmhl.html

[R42] 输入重定向
来源：http://hz.tianlin.xyz/gtynkqdmax.html

wc -l < a.txt
来源：http://hz.zhongyouzk.top/gtovagvgao.html

[R43] 按名字查找文件
来源：http://hz.sxryk.cn/gtvvnvdcuh.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtcmuyppuz.html

[R44] 按修改时间查找
来源：http://hz.xuanzx.com/gtbbzkthcx.html

find . -mtime -7 -type f
来源：http://hz.jqgufenzy.top/gtcsmwwraj.html

[R45] 批量删除
来源：http://hz.jqgufenzy.top/gtagtwjrpp.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtxojgppct.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gtcjwruvwe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtljkqdeqp.html

[R47] sed 单行替换
来源：http://hz.fengsongda.top/gtoroymeys.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.feifeiyinyue.top/gtstjhibox.html

[R48] awk 取指定列
来源：http://hz.kuanghao11.cn/gtrxacxagp.html

awk '{print $1, $3}' a.txt
来源：http://hz.hongshengwenyu.top/gtapmebwcu.html

[R49] awk 带条件
来源：http://hz.iojbl.cn/gtqbqhdzvl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.0kj1m.cn/gtzdrjkfbe.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtlqdplrab.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ehwqpu.com/gtmoajghsv.html

[R51] 排序去重取前几
来源：http://hz.zhijiandao.cn/gtdorjggmz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xuetiantiany.cn/gtzqzfolon.html

[R52] 统计行数
来源：http://hz.jinqigufen.top/gtxbhcpgth.html

wc -l a.txt
来源：http://hz.cucudq.cn/gtwtbqlbwx.html

[R53] 查看文件头与实时尾
来源：http://hz.hnqzz.top/gttsfgsvrj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhixingplan.top/gtpwrkqjds.html

[R54] 比较两个文件
来源：http://hz.wangdashe.top/gtidvtxupj.html

diff a.txt b.txt
来源：http://hz.sxryk.cn/gtbeonnddb.html

[R55] 压缩与解压
来源：http://hz.fengsongda.top/gtggptjoyr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxinkj.top/gtptelzdui.html

[R56] 远程拷贝
来源：http://hz.fzhhl.top/gthjytlble.html

scp file user@host:/path/
来源：http://hz.xziqi.cn/gtzakgbkgk.html

[R57] 远程执行命令
来源：http://hz.xziqi.cn/gtmjrfppor.html

ssh user@host 'uptime'
来源：http://hz.zhoulong.xyz/gtmqkxhdtp.html

[R58] 下载文件
来源：http://hz.sweek.top/gtpzhhajvb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtyjxxdklt.html

[R59] 发 POST JSON
来源：http://hz.dianchejie.cn/gtgxfirqow.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.iojbl.cn/gtvqhphjfz.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gthdnxgyvl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtrkzqyxnx.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gttaoadtje.html

df -h;  du -sh *
来源：http://hz.snrcjt.cn/gtqwbvyoph.html

[R62] 找最占空间的文件
来源：http://hz.dianchejie.cn/gtvuzsmvbx.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtyjdtfibi.html

[R63] 内存与进程
来源：http://hz.dianchejie.cn/gtsvjmvpdd.html

free -h;  ps aux | grep nginx
来源：http://hz.dashuyun.cn/gtqgqqeuuz.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtnxtfuaww.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pengpengdd.cyou/gtytodpuvd.html

[R65] 查看端口占用
来源：http://hz.dashuyun.cn/gtuhtouezs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xinyue.icu/gtrrdhuakz.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gtgcajcyun.html

crontab -e;  crontab -l
来源：http://hz.svipenyu.cn/gtfajdhpbv.html

[R67] 生成随机十六进制串
来源：http://hz.hnqzz.top/gtiwqknalf.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtwljuhadw.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gtwupeziip.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtwvyhsrel.html

[R69] 生成随机密码
来源：http://hz.zhongyouzk.top/gtqacxuawd.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhiwuduotai.top/gtgmmqhqnz.html

[R70] 时间戳与互转
来源：http://hz.ybcxt.top/gtxdesqdho.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtqnrbwpsh.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtvxywfxgx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yangfankeji.com/gtfndyevik.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtaaxzgrdm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nanxinkj.top/gtwwpzovfp.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gttvooainl.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtkgdodney.html

[R74] 批量重命名
来源：http://hz.dashuyun.cn/gtnipmvkpd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuxming.cn/gtavonziuq.html

[R75] 导出环境变量
来源：http://hz.jiagoushi.top/gtaokmvsry.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigufen.top/gtzsgoxdet.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangtech.top/gtgbwtbpho.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtudzxsays.html

[R77] 读取用户输入
来源：http://hz.hywenlv.cn/gtcvautehh.html

read -rp "请输入: " ans
来源：http://hz.shanyushiyangkeji.top/gtxeumefgu.html

[R78] 交互式菜单
来源：http://hz.tanke756.top/gtbtzricfv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jlsjyb.cn/gtnjysmbyf.html

[R79] 解析命令行选项
来源：http://hz.zhongyouzk.top/gtrpuwkbel.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtalvfhjzt.html

[R80] 查看脚本执行耗时
来源：http://hz.tian-w.cn/gtuoeocmqs.html

time ./run.sh
来源：http://hz.birdmap.top/gtfxsvbvbf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgwodgidv.html

S. C / C++ 专题
来源：http://hz.zhongyouzk.top/gtvoyellbm.html

================================================================================
来源：http://hz.gogol.net.cn/gtiznyltam.html

[S01] C：Hello World
来源：http://hz.yueranfly.top/gtpyxjagpm.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtjpodspef.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gthwaogoja.html

[S02] C：变量与格式化输出
来源：http://hz.hfpthk.cn/gtdnghpzot.html

int a = 10; printf("%d\n", a);
来源：http://hz.pengpengdd.cyou/gtqmczgczg.html

[S03] C：读入整数
来源：http://hz.0kj1m.cn/gtbfjerwdg.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gtsltplnob.html

[S04] C：字符串复制
来源：http://hz.hammf.cn/gtjdctrpge.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gtzpsaiwio.html

[S05] C：字符串长度
来源：http://hz.316326.xyz/gtsfbotrtn.html

strlen(s)
来源：http://hz.cqqwz.cn/gtexlcjrvz.html

[S06] C：字符串比较
来源：http://hz.zhaomingkeji.xyz/gtupwvwlts.html

strcmp(a, b) == 0
来源：http://hz.birdmap.top/gtcgorowuo.html

[S07] C：数组遍历求和
来源：http://hz.shuidangran.top/gtpoyxkntj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhiwuduotai.top/gtakxcpjlp.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtjjbaukgw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtfmqtrvmm.html

[S09] C：结构体定义与初始化
来源：http://hz.jlsjyb.cn/gtfvfxsysy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnxiangtu.top/gtwybdirbh.html

[S10] C：指针与解引用
来源：http://hz.yongpay.top/gtzvodjmmw.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtdlvwwnjr.html

[S11] C：逐行读文件
来源：http://hz.nwbrower.top/gtsgmperom.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gtqqozjkdr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sysykeji.top/gtrijfeufc.html

fclose(f);
来源：http://hz.nanxinkj.top/gtltadming.html

[S12] C：写文件
来源：http://hz.tanke756.top/gtwflyirok.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hongshengwenyu.top/gtwnlwxeun.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gtxmfoxauh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gtocnprgyj.html

[S14] C：枚举
来源：http://hz.9152youxi.cn/gtkblcgsss.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daxiang520.top/gtahxjcski.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gtjrnyscws.html

(double) a / b
来源：http://hz.hywenlv.cn/gtcicmrfto.html

[S16] C：位操作置位
来源：http://hz.meibo888.top/gtslmwuhez.html

x |= (1 << 3);
来源：http://hz.guowangkeji.top/gtcamqyvkm.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtnayatdon.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxuanxn.top/gtjujjblqq.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtwfcdxtbw.html

int main(int argc, char **argv)
来源：http://hz.cqqwz.cn/gtjkpfqbdm.html

[S19] C：快速排序
来源：http://hz.yongpay.top/gttdxgsuzy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.birdmap.top/gtauhoxgrk.html

[S20] C：二分查找
来源：http://hz.nanxuanxn.top/gtszonfpey.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtsbrirrcd.html

[S21] C：字符类别判断
来源：http://hz.jlsjyb.cn/gtjvfrcjoe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtgjnuylcw.html

[S22] C：字符串转数字
来源：http://hz.yj20258888.top/gtayzzoicd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtkbpzfjvg.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtdcutlbsp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xylfe.cn/gtwcjypddy.html

[S24] C：获取本地时间
来源：http://hz.ybcxt.top/gtxzxewaik.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gtshjwalys.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gtpzvjhfni.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtugzfquec.html

[S26] C：内存清零
来源：http://hz.cucudq.cn/gtyxtlylfh.html

memset(a, 0, sizeof a);
来源：http://hz.hfpthk.cn/gtvqrwuuvf.html

[S27] C：定义常量
来源：http://hz.zhiwuduotai.top/gtvdmmbmhy.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtmmqntxmw.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtmktfxbzt.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtwmgcwrse.html

[S29] C：变参函数
来源：http://hz.tanke756.top/gtxkqjaftq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.dashuyun.cn/gtbokrjmax.html

[S30] C：头文件保护
来源：http://hz.52xcode.cn/gtmazxmmdr.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtngspampf.html

#define X_H
来源：http://hz.ydjk.org.cn/gtdatmkllb.html

#endif
来源：http://hz.havefunace.top/gtvnoolygl.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gtcjihtjti.html

#include <iostream>
来源：http://hz.fzhhl.top/gtrbzxkmqj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gthmzoidsc.html

[S32] C++：字符串
来源：http://hz.redwolf501.top/gtodvpuyya.html

std::string s = "hi";  s += "!";
来源：http://hz.ivvv.top/gtfjujwxrc.html

[S33] C++：vector 增删
来源：http://hz.chenjidiqi.icu/gttzgpolbn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtzazjslwv.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtopqtkqss.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.smart0.xyz/gtowsvionk.html

[S35] C++：map
来源：http://hz.zhoulong.xyz/gtagxxxunh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtjdenvhxy.html

[S36] C++：unordered_map
来源：http://hz.bjfxy.top/gtdbqnrzkh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtyydayeai.html

[S37] C++：set
来源：http://hz.shangyingyoupin.top/gtmqgwytcd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shzxlz.cn/gtexaudvnd.html

[S38] C++：排序
来源：http://hz.yonumen.top/gtoiivyysg.html

std::sort(v.begin(), v.end());
来源：http://hz.vqdsnc.cn/gtueyxyeze.html

[S39] C++：自定义比较器排序
来源：http://hz.yueranfly.top/gtkeilwpui.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guannengcc.top/gtupnwcnhr.html

[S40] C++：查找元素
来源：http://hz.xziqi.cn/gtfhezlsxm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gzhubu.top/gtxyvrhzxh.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gtciostoop.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yvedp.cn/gtyiokgfoe.html

[S42] C++：继承与虚函数
来源：http://hz.jyoumei.cn/gtdlorykpa.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gthwezlhww.html


<!-- 参考信息 -->