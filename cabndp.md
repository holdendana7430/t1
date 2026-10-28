代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtqmsbsryg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ybcxt.top/gtmdvpwomh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtdtbttcsy.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtezdctpec.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.c1oappe.top/gtpmfwgeew.html

[Q58] 累计求和
来源：http://hz.shuidangran.top/gtibndanex.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.aizwys.cn/gtncdadxhr.html

[Q59] 分组内累计
来源：http://hz.chenzaomai.com/gtmbqksvhd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangshuangyany.cn/gtpljvdimf.html

[Q60] 取上一行 / 下一行
来源：http://hz.gotoacloud.top/gtsfhagibt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gthfaacegs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgfzy.top/gtxgsdbghm.html

[Q61] 移动平均
来源：http://hz.tanke756.top/gtgzlhrmcy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuanzx.com/gtvyyxdabw.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gttamqillw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hnqzz.top/gtwweyxjyc.html

[Q63] 开启事务
来源：http://hz.gzhubu.top/gtddgnhtal.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gtobsqluqt.html

[Q64] 提交事务
来源：http://hz.xuanzx.com/gtwxobwqlq.html

COMMIT;
来源：http://hz.zhijiandao.cn/gtviukiwrr.html

[Q65] 回滚事务
来源：http://hz.nanxuanxn.top/gtluboflkp.html

ROLLBACK;
来源：http://hz.yueranfly.top/gthjthwdgy.html

[Q66] 行锁查询
来源：http://hz.sweek.top/gtlafjfwms.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zycfv.cn/gtgpunrfej.html

[Q67] 设置隔离级别
来源：http://hz.xuetiantiany.cn/gtlrdcqbqz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cheryme.top/gtppkhskmg.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtkeraqaig.html

SAVEPOINT sp1;
来源：http://hz.cdnleiting.top/gtvppcauhe.html

ROLLBACK TO sp1;
来源：http://hz.kuanghao11.cn/gtsdqwsgip.html

[Q69] 查看执行计划
来源：http://hz.c1oappe.top/gtdveaguvf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnxiangtu.top/gtmfrqvjbu.html

[Q70] 更新统计信息
来源：http://hz.chenzaomai.com/gterbzagrt.html

ANALYZE TABLE users;
来源：http://hz.daxiang520.top/gtjjsedkqs.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gtsbmmadqc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guannengcc.top/gtnbjwrhjf.html

[Q72] 查看索引
来源：http://hz.xinyue.icu/gtenqrnsyb.html

SHOW INDEX FROM users;
来源：http://hz.gzhubu.top/gtcucpemux.html

[Q73] 查看表状态
来源：http://hz.jianghu66.top/gtpzdlvnvy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nwbrower.top/gtbrjgnfkb.html

[Q74] 强制使用索引
来源：http://hz.kuanghao11.cn/gtfdrvwabs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.c1oappe.top/gttumsnzgz.html

[Q75] 日期格式化
来源：http://hz.zhengqikj.top/gtydfoinso.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gtmpuyysxm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtpggxiwux.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtqjgmnogt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydzc1.top/gtifixxhxz.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtsxrejdpp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gttzhlbfuo.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gttnwuxfay.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.0kj1m.cn/gtlckyjxwp.html

[Q79] 字符串拼接
来源：http://hz.gaohongyu789.top/gtfedcvpgo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.svipenyu.cn/gtrmmdexyj.html

[Q80] 字符串截取
来源：http://hz.chenlongwang.top/gtuxdpbvwf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sweek.top/gtdgzdqnuv.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtbtfhupyc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yangfankeji.com/gtsznwiiuf.html

[Q82] 字符长度与字节长度
来源：http://hz.daxiang520.top/gtnwciwdfw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yangfankeji.com/gthqoewkfs.html

[Q83] 大小写转换
来源：http://hz.cucudq.cn/gtjwvpntzi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zdqjudy.top/gtxgcfchhx.html

[Q84] 去除首尾空格
来源：http://hz.yueranfly.top/gtxcqxcnsk.html

SELECT TRIM(name) FROM users;
来源：http://hz.cdnleiting.top/gthjjtihzn.html

[Q85] 数值取整
来源：http://hz.yj202588.top/gtkwnqhtdl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.316326.xyz/gtlmcjwawd.html

[Q86] 读取 JSON 字段
来源：http://hz.guannengcc.top/gtvmsclaaq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangdashe.top/gtbabeyndh.html

[Q87] JSON 字段做条件
来源：http://hz.smart0.xyz/gtcmegozfd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnxiangtu.top/gtfxgbcvjm.html

[Q88] 行转列（条件聚合）
来源：http://hz.jyoumei.cn/gtkvsbwdwi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtvwfyrrcs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.mhx1999.top/gtqwmkrcmu.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtwgasgvrz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.redwolf501.top/gtiquwthav.html

[Q90] 生成序号列
来源：http://hz.jqgufenzy.top/gttimvqlma.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhixingplan.top/gtdhfwmwcy.html

================================================================================
来源：http://hz.jianghu66.top/gtoxobrglm.html

R. Bash 专题
来源：http://hz.nanxinkj.top/gtmragvcdx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwjzffiwd.html

[R01] shebang 与严格模式
来源：http://hz.xingfuxueyuan.xyz/gtjhhjrerh.html

#!/usr/bin/env bash
来源：http://hz.0kj1m.cn/gtiumxbrbw.html

set -euo pipefail
来源：http://hz.jiagoushi.top/gtahvfsvwg.html

[R02] 变量赋值与使用
来源：http://hz.yvedp.cn/gtldcoyqrx.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gtnmgyuzcg.html

[R03] 只读变量
来源：http://hz.zhixingplan.top/gtsehuonpg.html

readonly PI=3.14
来源：http://hz.mhx1999.top/gtxqgpnjwc.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtalemolzu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hywenlv.cn/gtrawfieug.html

[R05] 参数默认值
来源：http://hz.yuanzhike.top/gtheyhdzcg.html

name="${1:-default}"
来源：http://hz.cucudq.cn/gtplgdxhec.html

[R06] 判断命令是否存在
来源：http://hz.mhx1999.top/gtatnjhipq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guowangkeji.top/gtmdrnyxor.html

[R07] if 判断文件
来源：http://hz.dashuyun.cn/gtxucoqjgk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sysykeji.top/gtysazvwiw.html

[R08] 数值比较
来源：http://hz.svipenyu.cn/gtbbbblrqd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fzhhl.top/gtaagohvzm.html

[R09] 字符串比较
来源：http://hz.quarkkingdee.top/gtjugxefzw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtpngwmwpx.html

[R10] 正则匹配
来源：http://hz.shuidangran.top/gtfkgkrsiv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yvedp.cn/gthxcuntdo.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtzbwirnyb.html

case "$1" in
来源：http://hz.nanxuanxn.top/gtmprvaqoy.html

start) echo "启动" ;;
来源：http://hz.sweek.top/gtuerxopam.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gtsitmbxvj.html

*)     echo "未知命令" ;;
来源：http://hz.quarkkingdee.top/gtmjiqizqd.html

esac
来源：http://hz.iojbl.cn/gtgllkzjzr.html

[R12] for 遍历文件
来源：http://hz.jinyuanbaomall.cn/gtbrlkloky.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtysxxqehf.html

[R13] for 计数循环
来源：http://hz.iojbl.cn/gteybzautn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.daxiang520.top/gtjaqoxiwt.html

[R14] C 风格 for
来源：http://hz.cashguo.top/gtwrrpkwac.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangdashe.top/gthpuowhrf.html

[R15] while 逐行读文件
来源：http://hz.yuanzhike.top/gtygwdrrjm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtgkfmmoqk.html

[R16] until 等待条件
来源：http://hz.316326.xyz/gtyzisdksp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.bjfxy.top/gtwluwvilw.html

[R17] 数组定义与取值
来源：http://hz.jqgfzy.top/gtybyabsxh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dianchejie.cn/gtkqtlzjfs.html

[R18] 遍历数组
来源：http://hz.guowangkeji.top/gtjpyjcjet.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.snrcjt.cn/gtituwzftk.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtidoiovde.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtcaqdjzjp.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtyoztrxfl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinghuilouyu.cn/gtqhqvcojx.html

[R21] 字符串长度
来源：http://hz.haohaochexian.top/gtoravyjxb.html

echo "${#s}"
来源：http://hz.jianghu66.top/gtchjxgjtb.html

[R22] 截取子串
来源：http://hz.tanke756.top/gtoskplchp.html

echo "${s:0:5}"
来源：http://hz.cdnleiting.top/gtnfxkhemo.html

[R23] 字符串替换
来源：http://hz.jiagoushi.top/gtuolwuizf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtogxgtexm.html

[R24] 大小写转换
来源：http://hz.hammf.cn/gtzeujqqiw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtoyajpwqj.html

[R25] 去后缀 / 去前缀
来源：http://hz.316326.xyz/gtwozqvlei.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgfzy.top/gtrxhyaucx.html

[R26] 命令替换
来源：http://hz.shangyingyoupin.top/gtejogicle.html

now=$(date +%F); echo "$now"
来源：http://hz.xuanzx.com/gtczrtbtfy.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtkmutzzsd.html

echo $((1 + 2 * 3))
来源：http://hz.smart0.xyz/gtuaycqayq.html

[R28] 浮点运算
来源：http://hz.sweek.top/gtmrplypfe.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtivflpabk.html

[R29] 定义函数
来源：http://hz.cqqwz.cn/gtztgjlrnw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gzhubu.top/gtrdmzajgx.html

[R30] 函数返回状态码
来源：http://hz.daxiang520.top/gtfxjvtawj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.bjfxy.top/gtldgboawe.html

[R31] 局部变量
来源：http://hz.hywenlv.cn/gtebcoakzj.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtikidnhgh.html

[R32] 参数个数校验
来源：http://hz.yanxiufei.cn/gtmxzfdvaj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shzxlz.cn/gtypgxymir.html

[R33] 捕获错误并提示行号
来源：http://hz.jinghuilouyu.cn/gtilzbnasm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ppjwa.cn/gtfogqmiix.html

[R34] 退出时清理
来源：http://hz.shanyushiyangkeji.top/gtvznjodvj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtmetpuioo.html

[R35] 后台执行并等待
来源：http://hz.zhongyouzk.top/gtsuqriwoq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gtldgzdnvw.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtuxafheja.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yanxiufei.cn/gtidnmlpxs.html

[R37] 把输出赋给变量
来源：http://hz.cucudq.cn/gtnqkzbiki.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtrniptlqu.html

[R38] 管道串联
来源：http://hz.kuanghao11.cn/gtxellxasz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhaomingkeji.xyz/gtmryuwhzn.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtqbwphzsi.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtylkexbnd.html

[R40] 追加写日志
来源：http://hz.yueranfly.top/gtvmpybnsi.html

echo "log" >> out.log
来源：http://hz.xziqi.cn/gtjltokcwu.html

[R41] 丢弃输出
来源：http://hz.daxiang520.top/gtfiqdbsra.html

cmd >/dev/null 2>&1
来源：http://hz.zhixingplan.top/gtssbuwplw.html

[R42] 输入重定向
来源：http://hz.sufxvd.cn/gtvzzgznaf.html

wc -l < a.txt
来源：http://hz.gotoacloud.top/gtodpvnyqu.html

[R43] 按名字查找文件
来源：http://hz.hywenlv.cn/gtntsujfqu.html

find . -name "*.log" -type f
来源：http://hz.jiagoushi.top/gtouiseaxm.html

[R44] 按修改时间查找
来源：http://hz.cdnleiting.top/gteoowgjgt.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtbtnaappw.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtejfhjfdi.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtyzzxxnxw.html

[R46] 递归替换文件内容
来源：http://hz.hnqzz.top/gtbbevyeof.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtnupvyiyr.html

[R47] sed 单行替换
来源：http://hz.pycfn.com/gtcmzscmtu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tianlin.xyz/gtcsyihwxn.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtfotfeyuf.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gtudvffbhq.html

[R49] awk 带条件
来源：http://hz.zhixingplan.top/gtgghjnelx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hammf.cn/gtcprnpieq.html

[R50] awk 求和
来源：http://hz.xinyue.icu/gthfghvvwn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtjxnmzueq.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtaipflzfd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gaohongyu789.top/gtgqpcwsyg.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gtvkolzjir.html

wc -l a.txt
来源：http://hz.gzhubu.top/gtibdpiykw.html

[R53] 查看文件头与实时尾
来源：http://hz.gotoacloud.top/gtynuhcqye.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yongpay.top/gtcvxkloln.html

[R54] 比较两个文件
来源：http://hz.yj202588.top/gthtpgifsv.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gtlidrmmni.html

[R55] 压缩与解压
来源：http://hz.yueranfly.top/gtwirqyiqu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.mhx1999.top/gtcyrxbrms.html

[R56] 远程拷贝
来源：http://hz.zhengqikj.top/gtokqhcncr.html

scp file user@host:/path/
来源：http://hz.ydjk.org.cn/gtephybuul.html

[R57] 远程执行命令
来源：http://hz.sysykeji.top/gtuvlvqypg.html

ssh user@host 'uptime'
来源：http://hz.jqgufenzy.top/gtetvfywdz.html

[R58] 下载文件
来源：http://hz.dashuyun.cn/gtbhvjoymc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.0kj1m.cn/gtlpjykxgp.html

[R59] 发 POST JSON
来源：http://hz.shangyingyoupin.top/gtkgypiktq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.andypj.xyz/gttcpnlrzy.html

[R60] 只看 HTTP 状态码
来源：http://hz.0kj1m.cn/gtmxjzxplm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtdwhkayae.html

[R61] 磁盘占用
来源：http://hz.xinyue.icu/gtrjtgnffw.html

df -h;  du -sh *
来源：http://hz.ybcxt.top/gtlssryxtj.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtukwlgzka.html

du -ah . | sort -rh | head -10
来源：http://hz.ybcxt.top/gtsicguvhd.html

[R63] 内存与进程
来源：http://hz.redwolf501.top/gtvlanccsa.html

free -h;  ps aux | grep nginx
来源：http://hz.0kj1m.cn/gtiwkqrali.html

[R64] 结束进程
来源：http://hz.chenjidiqi.icu/gtrvhamufc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtnsoaxois.html

[R65] 查看端口占用
来源：http://hz.mhx1999.top/gthlrxcfhz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.9152youxi.cn/gtdgqzqnjq.html

[R66] 定时任务
来源：http://hz.quarkkingdee.top/gtpgjlldyx.html

crontab -e;  crontab -l
来源：http://hz.bjfxy.top/gtpkqkgzjy.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtojxjloae.html

openssl rand -hex 16
来源：http://hz.fzhhl.top/gtfeajdpjn.html

[R68] 计算文件校验值
来源：http://hz.9152youxi.cn/gtcljmgtzr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxinkj.top/gtxsotfgrs.html

[R69] 生成随机密码
来源：http://hz.yj20258.top/gtlgpgodiq.html

head -c 16 /dev/urandom | base64
来源：http://hz.cucudq.cn/gtujbhlfyi.html

[R70] 时间戳与互转
来源：http://hz.jiagoushi.top/gtwbzatfwv.html

date +%s;  date -d @1700000000
来源：http://hz.jyoumei.cn/gtmooecqyq.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtdaniomka.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtuoimefeq.html

[R72] 等待端口就绪
来源：http://hz.guowangkeji.top/gtjkaflkfg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dianchejie.cn/gtkjvjtytc.html

[R73] 分割大日志
来源：http://hz.meibo888.top/gtlfetkcrf.html

split -l 1000 big.log part_
来源：http://hz.aizwys.cn/gtqwhivtnc.html

[R74] 批量重命名
来源：http://hz.yueranfly.top/gtpxbnwevs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.havefunace.top/gtsmscmkdd.html

[R75] 导出环境变量
来源：http://hz.feifeiyinyue.top/gthewpcwcq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jqgfzy.top/gtnlchgroz.html

[R76] 使用临时文件
来源：http://hz.haohaochexian.top/gtvdlwnntk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtoqujpqqs.html

[R77] 读取用户输入
来源：http://hz.haohaochexian.top/gtmpjrpqsj.html

read -rp "请输入: " ans
来源：http://hz.hywenlv.cn/gtyvdfqymw.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gttsmzgban.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtnbihhuql.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gtiiqqqhin.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cdnleiting.top/gtokcdjfyv.html

[R80] 查看脚本执行耗时
来源：http://hz.nwbrower.top/gtfthrdpwt.html

time ./run.sh
来源：http://hz.jlsjyb.cn/gtvycvqsrb.html

================================================================================
来源：http://hz.yuxming.cn/gtkxopcxin.html

S. C / C++ 专题
来源：http://hz.yongpay.top/gtockhdvzm.html

================================================================================
来源：http://hz.jqgfzy.top/gthxefnfwd.html

[S01] C：Hello World
来源：http://hz.pycfn.com/gtoqxftkwi.html

#include <stdio.h>
来源：http://hz.quarkkingdee.top/gtwsesclhp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtwueyvoyg.html

[S02] C：变量与格式化输出
来源：http://hz.cqqwz.cn/gtmieyiavo.html

int a = 10; printf("%d\n", a);
来源：http://hz.hywenlv.cn/gtkbmsmgip.html

[S03] C：读入整数
来源：http://hz.wangdashe.top/gtheasjejl.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gtcgkjzidc.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gttiosqlem.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhoulong.xyz/gtxlvvobfy.html

[S05] C：字符串长度
来源：http://hz.dashuyun.cn/gtbouvbvaa.html

strlen(s)
来源：http://hz.hysaishi.cn/gtwvrnxeiw.html

[S06] C：字符串比较
来源：http://hz.jinghuilouyu.cn/gtjahuvtdx.html

strcmp(a, b) == 0
来源：http://hz.ydjk.org.cn/gtxbdolnnj.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gttfpemdkn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.meibo888.top/gtpespklzw.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtxbygzkku.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ybcxt.top/gtwtvgktfz.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtnmszflda.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daria6918.cn/gtooankiql.html

[S10] C：指针与解引用
来源：http://hz.316326.xyz/gtccveghdw.html

int *p = &a;  *p = 5;
来源：http://hz.cashguo.top/gtgsacgouk.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtcyeanwvl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtdivrwqjl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtqfcmfvzd.html

fclose(f);
来源：http://hz.xylfe.cn/gtpcsynvfw.html

[S12] C：写文件
来源：http://hz.shanyushiyangkeji.top/gtxomjmgmy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xylfe.cn/gtvzgrvqre.html

[S13] C：宏定义
来源：http://hz.yanxiufei.cn/gtewvfwaec.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shanyushiyangkeji.top/gtiucebsga.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtltpxsvni.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxinkj.top/gtphmsevxh.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gtgiccumzd.html

(double) a / b
来源：http://hz.andypj.xyz/gtqpqwxzpx.html

[S16] C：位操作置位
来源：http://hz.pycfn.com/gtgczddghp.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gtwwjowmik.html

[S17] C：安全拼接字符串
来源：http://hz.jqgfzy.top/gtnueaoeqr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gtgbtemytn.html

[S18] C：命令行参数
来源：http://hz.quarkkingdee.top/gtwjxjjtzg.html

int main(int argc, char **argv)
来源：http://hz.jinghuilouyu.cn/gtyeeexjhv.html

[S19] C：快速排序
来源：http://hz.hfpthk.cn/gtfkfxrozu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtgjmfggiu.html

[S20] C：二分查找
来源：http://hz.ppjwa.cn/gtyxlhkmaq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtfcjfwlhy.html

[S21] C：字符类别判断
来源：http://hz.yueranfly.top/gtrwjvclay.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sufxvd.cn/gtnabxgjyx.html

[S22] C：字符串转数字
来源：http://hz.guannengcc.top/gtwkchzati.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hnqzz.top/gtzvgpnscp.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gtseikhvzz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.redwolf501.top/gterhepegg.html

[S24] C：获取本地时间
来源：http://hz.zhixingplan.top/gtogolzcda.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hnxiangtu.top/gtjnzyctqh.html

[S25] C：内存拷贝
来源：http://hz.zycfv.cn/gtqfvtvzcs.html

memcpy(dst, src, n);
来源：http://hz.jinghuilouyu.cn/gtjhvonsju.html

[S26] C：内存清零
来源：http://hz.sysykeji.top/gtxwncffna.html


<!-- 参考信息 -->