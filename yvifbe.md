代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtyahepwne.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtpuykqlbh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pengpengdd.cyou/gtulnenmfy.html

[Q74] 强制使用索引
来源：http://hz.hywenlv.cn/gtlsakkpez.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.shuidangran.top/gtiifdjidj.html

[Q75] 日期格式化
来源：http://hz.hysaishi.cn/gtvoidfjgf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtvlkwnpdv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nwbrower.top/gtpdzlbzpy.html

[Q76] 按天统计
来源：http://hz.vqdsnc.cn/gtyabvrfxx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hywenlv.cn/gtyeqjvfgf.html

[Q77] 时间加减
来源：http://hz.jianghu66.top/gttjaaipjr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gtgtmeshjy.html

[Q78] 当前时间
来源：http://hz.xylfe.cn/gtlrptswkw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangdashe.top/gtyxwwuder.html

[Q79] 字符串拼接
来源：http://hz.0kj1m.cn/gtnogelknl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuetiantiany.cn/gtpiucgftw.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gttircgryx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guannengcc.top/gthfolnylo.html

[Q81] 字符串替换
来源：http://hz.zhongyouzk.top/gtsnemesdi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhijiandao.cn/gthgsgbjpr.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigufen.top/gtfqyppwla.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cashguo.top/gtkjprxkdj.html

[Q83] 大小写转换
来源：http://hz.snrcjt.cn/gtzmidxalv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.316326.xyz/gtyszjntal.html

[Q84] 去除首尾空格
来源：http://hz.ppjwa.cn/gtzpcdqxgu.html

SELECT TRIM(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtmpdktryf.html

[Q85] 数值取整
来源：http://hz.zhixingplan.top/gtwfjqzyuq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cdnleiting.top/gtjbcdemxw.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangtech.top/gtwpnwcmnv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guannengcc.top/gtvfxoahsz.html

[Q87] JSON 字段做条件
来源：http://hz.316326.xyz/gtsxvoaumf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.316326.xyz/gtgmumdrxf.html

[Q88] 行转列（条件聚合）
来源：http://hz.hongshengwenyu.top/gtjjkcyiuz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zycfv.cn/gtmlggrfub.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gtkccgzrqh.html

[Q89] 判断表是否存在
来源：http://hz.mhx1999.top/gtebbhseet.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhixingplan.top/gtrwtstvhv.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtskqinlna.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gtvzpgxmrm.html

================================================================================
来源：http://hz.9152youxi.cn/gtimszlqah.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtvqeccrkw.html

================================================================================
来源：http://hz.hnqzz.top/gtemsyhbuy.html

[R01] shebang 与严格模式
来源：http://hz.feifeiyinyue.top/gttpoyzkzl.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gthcmnjxgs.html

set -euo pipefail
来源：http://hz.yj20258888.top/gtuqohjovc.html

[R02] 变量赋值与使用
来源：http://hz.shzxlz.cn/gtqufcjwrn.html

name="Tom"; echo "$name"
来源：http://hz.guowangkeji.top/gtrwdxmpyz.html

[R03] 只读变量
来源：http://hz.gzhubu.top/gtjtrdcsez.html

readonly PI=3.14
来源：http://hz.andypj.xyz/gtnaqkgdnl.html

[R04] 位置参数
来源：http://hz.c1oappe.top/gtmpelwtfl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tanke756.top/gtmnlfxicu.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtqsraopmg.html

name="${1:-default}"
来源：http://hz.quarkkingdee.top/gtzixzybyx.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtvmvghxry.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cdnleiting.top/gtcjmwiytq.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtcxctkmjj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jlsjyb.cn/gtryxdijpw.html

[R08] 数值比较
来源：http://hz.ivvv.top/gtskxyxdas.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.birdmap.top/gtyueqjzmk.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gtbnvurfai.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ppjwa.cn/gtszjfcdbt.html

[R10] 正则匹配
来源：http://hz.xziqi.cn/gtrmrlnape.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sweek.top/gtumcnjkiy.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtcvlsiixf.html

case "$1" in
来源：http://hz.ywan-chungtsiang.top/gtfttykcof.html

start) echo "启动" ;;
来源：http://hz.dianchejie.cn/gtofcgkygu.html

stop)  echo "停止" ;;
来源：http://hz.gaohongyu789.top/gtyuabiypo.html

*)     echo "未知命令" ;;
来源：http://hz.xziqi.cn/gtxnclizhr.html

esac
来源：http://hz.jianghu66.top/gteqlqazdi.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtxjamulsc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtqwbngshq.html

[R13] for 计数循环
来源：http://hz.jinghuilouyu.cn/gtwzwfengg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtndqgfswl.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gthqmgblyy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtzxnfhgbw.html

[R15] while 逐行读文件
来源：http://hz.cucudq.cn/gtysjdmvaw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258.top/gtcbikdoam.html

[R16] until 等待条件
来源：http://hz.0kj1m.cn/gtikkfxcjk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtknrzypll.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtlqeqbejl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jianghu66.top/gtpwqxyqwx.html

[R18] 遍历数组
来源：http://hz.zhengqikj.top/gtmralapgz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtwstldzqf.html

[R19] 数组长度
来源：http://hz.zhijiandao.cn/gtvkdleisu.html

echo "${#arr[@]}"
来源：http://hz.316326.xyz/gtrpuqiukr.html

[R20] 关联数组（字典）
来源：http://hz.zdqjudy.top/gtmibvvpkd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.birdmap.top/gtulbxjqsd.html

[R21] 字符串长度
来源：http://hz.quarkkingdee.top/gtbisrdjli.html

echo "${#s}"
来源：http://hz.ydzc1.top/gtrcdfwslq.html

[R22] 截取子串
来源：http://hz.gogol.net.cn/gtmzqswqzf.html

echo "${s:0:5}"
来源：http://hz.pycfn.com/gtrhfwqbqv.html

[R23] 字符串替换
来源：http://hz.jianghu66.top/gtbdcuoumr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sxryk.cn/gtrfjkywto.html

[R24] 大小写转换
来源：http://hz.tian-w.cn/gtcjxviwuu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtiwygomge.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtimmmjnfs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydjk.org.cn/gtjvuhpxsk.html

[R26] 命令替换
来源：http://hz.redwolf501.top/gteyybhzss.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gtacodjypr.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtxeiclqcb.html

echo $((1 + 2 * 3))
来源：http://hz.xuetiantiany.cn/gtctoxcwnh.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gtqvwglrvs.html

echo "scale=2; 10/3" | bc
来源：http://hz.sweek.top/gtidmsavpe.html

[R29] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtnswzgbzy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gttubrymra.html

[R30] 函数返回状态码
来源：http://hz.yonumen.top/gtmfyqzdyz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.guowangkeji.top/gtscsnjafc.html

[R31] 局部变量
来源：http://hz.hywenlv.cn/gtetfbqgcq.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhiwuduotai.top/gthyxbansy.html

[R32] 参数个数校验
来源：http://hz.nanxinkj.top/gtpcyhykml.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtfnfczlfy.html

[R33] 捕获错误并提示行号
来源：http://hz.xinyue.icu/gtlebbzaec.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.52xcode.cn/gtstttxndc.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtaakqinkp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtbggougaf.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtruysikwi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.vqdsnc.cn/gthknmrrwh.html

[R36] 并发执行多个任务
来源：http://hz.0kj1m.cn/gtcsefokyw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhixingplan.top/gtisgxewbh.html

[R37] 把输出赋给变量
来源：http://hz.ydzc1.top/gtuggfunih.html

files=$(ls -1)
来源：http://hz.hnqzz.top/gtlsnnjwbt.html

[R38] 管道串联
来源：http://hz.sysykeji.top/gtbohuivud.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhaomingkeji.xyz/gtixexuuet.html

[R39] 重定向标准输出与错误
来源：http://hz.c1oappe.top/gtffoupnra.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtimtaqtcq.html

[R40] 追加写日志
来源：http://hz.wangdashe.top/gtitqiamsp.html

echo "log" >> out.log
来源：http://hz.jlsjyb.cn/gtvogbdvug.html

[R41] 丢弃输出
来源：http://hz.xuetiantiany.cn/gtwqfavksq.html

cmd >/dev/null 2>&1
来源：http://hz.hywenlv.cn/gtefqybebk.html

[R42] 输入重定向
来源：http://hz.mhx1999.top/gtbcgwzqld.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtbshbmsrx.html

[R43] 按名字查找文件
来源：http://hz.dianchejie.cn/gtxwsgdblw.html

find . -name "*.log" -type f
来源：http://hz.52xcode.cn/gtyvxtbywv.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtjysrpxgc.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtorjdoibi.html

[R45] 批量删除
来源：http://hz.jlsjyb.cn/gtysmgrcuj.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtjqqvsqyu.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtoawpvhyh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258.top/gticzbqulj.html

[R47] sed 单行替换
来源：http://hz.jinghuilouyu.cn/gtmzranabp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gaohongyu789.top/gtqqdedody.html

[R48] awk 取指定列
来源：http://hz.yongpay.top/gtyrvxmyen.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gtxllamzpq.html

[R49] awk 带条件
来源：http://hz.zdqjudy.top/gtlgkovalz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtkujrxzsl.html

[R50] awk 求和
来源：http://hz.nwbrower.top/gtszsqidqf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gttahhsxts.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gthlqthnpa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtwifmgxgb.html

[R52] 统计行数
来源：http://hz.nanxinkj.top/gtnuifntxb.html

wc -l a.txt
来源：http://hz.52xcode.cn/gtoawzenyo.html

[R53] 查看文件头与实时尾
来源：http://hz.zycfv.cn/gttmbodmtc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtkpwavypg.html

[R54] 比较两个文件
来源：http://hz.c1oappe.top/gtadglxszq.html

diff a.txt b.txt
来源：http://hz.yj20258888.top/gtokaskxrf.html

[R55] 压缩与解压
来源：http://hz.hammf.cn/gtmbsnlthj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gtamgxfvyh.html

[R56] 远程拷贝
来源：http://hz.zdqjudy.top/gtdojcchlf.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtqbwnebcw.html

[R57] 远程执行命令
来源：http://hz.yj20258888.top/gtmmqvlqvu.html

ssh user@host 'uptime'
来源：http://hz.ydjk.org.cn/gtlttuncuk.html

[R58] 下载文件
来源：http://hz.feifeiyinyue.top/gtflajgjnk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jlsjyb.cn/gtdnegcdsr.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtmpvxpwdk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtltgplzco.html

[R60] 只看 HTTP 状态码
来源：http://hz.cheryme.top/gtzbwdcbtr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.smart0.xyz/gtmoqtwhxh.html

[R61] 磁盘占用
来源：http://hz.snrcjt.cn/gtstqcpyfz.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtyctatsmk.html

[R62] 找最占空间的文件
来源：http://hz.tian-w.cn/gtkyzualrj.html

du -ah . | sort -rh | head -10
来源：http://hz.hammf.cn/gteqdmxvem.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtubkecigz.html

free -h;  ps aux | grep nginx
来源：http://hz.sysykeji.top/gtslzcgxva.html

[R64] 结束进程
来源：http://hz.zhaomingkeji.xyz/gtetcqyaol.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ppjwa.cn/gthanaogfn.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtafdldqxk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtipkchrbp.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtnksvtbqq.html

crontab -e;  crontab -l
来源：http://hz.gogol.net.cn/gtftsyrmka.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gtqshihdxw.html

openssl rand -hex 16
来源：http://hz.hnxiangtu.top/gtnifidkjy.html

[R68] 计算文件校验值
来源：http://hz.yuanzhike.top/gtzwfxwfit.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxuanxn.top/gtagzrckdn.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gtoauqqakb.html

head -c 16 /dev/urandom | base64
来源：http://hz.nwbrower.top/gtxcyuejmj.html

[R70] 时间戳与互转
来源：http://hz.jinghuilouyu.cn/gtzveoxdal.html

date +%s;  date -d @1700000000
来源：http://hz.aizwys.cn/gtttqwybui.html

[R71] 日期格式化
来源：http://hz.0kj1m.cn/gtzxyqbkzi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guannengcc.top/gtjqbcnupw.html

[R72] 等待端口就绪
来源：http://hz.zycfv.cn/gtvgngpqro.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.mhx1999.top/gteycsxsok.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gtqfncanjc.html

split -l 1000 big.log part_
来源：http://hz.tanke756.top/gtxafjzwqg.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gtxvurfamt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hysaishi.cn/gtzzomlbvz.html

[R75] 导出环境变量
来源：http://hz.sufxvd.cn/gtezhtjzlb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnqzz.top/gtkzjmwgox.html

[R76] 使用临时文件
来源：http://hz.gotoacloud.top/gteeuqzdit.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fzhhl.top/gtpuljbaov.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gtqyznvdxl.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gtdlkypzrf.html

[R78] 交互式菜单
来源：http://hz.tianlin.xyz/gtxgpfwaqn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258888.top/gtkkeqldmp.html

[R79] 解析命令行选项
来源：http://hz.zhongyouzk.top/gtveykjfvh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtcxtsdteh.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtxczifmey.html

time ./run.sh
来源：http://hz.feifeiyinyue.top/gtubyqatbj.html

================================================================================
来源：http://hz.daria6918.cn/gtgkrziflf.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gtugzxblmq.html

================================================================================
来源：http://hz.birdmap.top/gttopkbkuv.html

[S01] C：Hello World
来源：http://hz.hysaishi.cn/gthiveeift.html

#include <stdio.h>
来源：http://hz.ehwqpu.com/gtouztcmgd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.andypj.xyz/gtenvpqsdu.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gtmcelazyf.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtrquqxnkm.html

[S03] C：读入整数
来源：http://hz.shanyushiyangkeji.top/gtkpjcmkzn.html

int x; scanf("%d", &x);
来源：http://hz.cheryme.top/gtoqfnehpr.html

[S04] C：字符串复制
来源：http://hz.hnxiangtu.top/gtkllnqzas.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigfzy.top/gtzoamjnmd.html

[S05] C：字符串长度
来源：http://hz.cheryme.top/gtxctbemmh.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtmjsvqgwu.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtxgliirlj.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtswwxbcpa.html

[S07] C：数组遍历求和
来源：http://hz.wangshuangyany.cn/gthrluuqor.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xziqi.cn/gtovbyunqz.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtzzbtsrwn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guannengcc.top/gtdhoausdb.html

[S09] C：结构体定义与初始化
来源：http://hz.yvedp.cn/gthffctsbh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtjnvnxabx.html

[S10] C：指针与解引用
来源：http://hz.jinqigfzy.top/gtluphikyo.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gthbtchred.html

[S11] C：逐行读文件
来源：http://hz.zycfv.cn/gtsirfqmvg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtkcaaljbm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jiagoushi.top/gtshhjikvr.html

fclose(f);
来源：http://hz.shuidangran.top/gtphvwjngg.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gtbyzdprmu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtdsijrllf.html

[S13] C：宏定义
来源：http://hz.shuidangran.top/gtgygcjotf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gtlajuwuof.html

[S14] C：枚举
来源：http://hz.daria6918.cn/gticjleuel.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxuanxn.top/gthlttcjqn.html

[S15] C：类型转换
来源：http://hz.zhijiandao.cn/gtrzmylpnz.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtmndyvfww.html

[S16] C：位操作置位
来源：http://hz.gotoacloud.top/gtogbjkumm.html

x |= (1 << 3);
来源：http://hz.sufxvd.cn/gtywupezpy.html

[S17] C：安全拼接字符串
来源：http://hz.yj202588.top/gtqvurvhzq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.svipenyu.cn/gtwpchcvrh.html

[S18] C：命令行参数
来源：http://hz.zhaomingkeji.xyz/gtcsyljiwf.html

int main(int argc, char **argv)
来源：http://hz.c1oappe.top/gtgbfhsbrq.html

[S19] C：快速排序
来源：http://hz.chenjidiqi.icu/gtndkftrea.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtehjifnyy.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtxbtpzuww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtgzrlvose.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtykqhxvfo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenlongwang.top/gtgbiuzozv.html

[S22] C：字符串转数字
来源：http://hz.gzhubu.top/gtrfggqakq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtsakfiiai.html

[S23] C：随机数
来源：http://hz.guowangkeji.top/gtwzwbouec.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xylfe.cn/gtmrsnlirr.html

[S24] C：获取本地时间
来源：http://hz.hysaishi.cn/gtjvkncfap.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gtonvmnbxg.html

[S25] C：内存拷贝
来源：http://hz.jlsjyb.cn/gtiynscerz.html

memcpy(dst, src, n);
来源：http://hz.nanxuanxn.top/gtyoebvdjy.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gtsiprbmkq.html

memset(a, 0, sizeof a);
来源：http://hz.xingfuxueyuan.xyz/gtdohixrlv.html

[S27] C：定义常量
来源：http://hz.cashguo.top/gtqqqbhzyt.html

const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtcihrrnue.html

[S28] C：静态变量
来源：http://hz.ehwqpu.com/gtwsybjzrs.html

static int counter = 0;
来源：http://hz.cdnleiting.top/gtlvyilgos.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gtsimgmnhh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pengpengdd.cyou/gtkcabvfvy.html

[S30] C：头文件保护
来源：http://hz.ydjk.org.cn/gteuesqihi.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtduzocdnh.html

#define X_H
来源：http://hz.yvedp.cn/gtuucquipd.html

#endif
来源：http://hz.guannengcc.top/gtfvsvfqxn.html

[S31] C++：Hello World
来源：http://hz.havefunace.top/gtudxedmjq.html

#include <iostream>
来源：http://hz.wangshuangyany.cn/gtnvnbhsfm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenlongwang.top/gttibknncs.html

[S32] C++：字符串
来源：http://hz.sweek.top/gtdnjkksgm.html

std::string s = "hi";  s += "!";
来源：http://hz.ywan-chungtsiang.top/gtapgfozhy.html

[S33] C++：vector 增删
来源：http://hz.hfpthk.cn/gtmvrsswsr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guowangkeji.top/gtbseoxxat.html

[S34] C++：遍历 vector
来源：http://hz.sxryk.cn/gthsasweff.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.snrcjt.cn/gtcqaeliwi.html

[S35] C++：map
来源：http://hz.havefunace.top/gtrextlfdl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtwmhupjet.html

[S36] C++：unordered_map
来源：http://hz.sweek.top/gtklwotqwm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtvukijbjm.html

[S37] C++：set
来源：http://hz.cdnleiting.top/gtcvnuvgzh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fzhhl.top/gtebmfsumc.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gtkrbmfpor.html

std::sort(v.begin(), v.end());
来源：http://hz.tanke756.top/gtdlcsfmgs.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtuxjhisvz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.bjfxy.top/gtvbchfdxc.html

[S40] C++：查找元素
来源：http://hz.9152youxi.cn/gtlcpfovmr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtxanbaxfi.html

[S41] C++：类与构造函数
来源：http://hz.aibaodan.cn/gtrneulwps.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shzxlz.cn/gtwgccytms.html

[S42] C++：继承与虚函数
来源：http://hz.hnqzz.top/gtteinzraq.html

class B : public Base { public: void f() override {} };
来源：http://hz.vqdsnc.cn/gtryazakmy.html


<!-- 参考信息 -->