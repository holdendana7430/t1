代发 wailian999

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtihqbgfiq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jianghu66.top/gtbztgmmlv.html

[Q45] EXISTS 判断存在
来源：http://hz.gaohongyu789.top/gtcnfisnop.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.kuanghao11.cn/gtjwjiobav.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhoulong.xyz/gtlmqgybpr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gtvltukunc.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtvpcmzrmu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtlzvmxvqo.html

[Q48] CTE 公用表表达式
来源：http://hz.smart0.xyz/gtsdhphbkw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yvedp.cn/gtaikjcomo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhengqikj.top/gtnglvlkiz.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gttzswaxas.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jiagoushi.top/gtkgszkxns.html

[Q50] 批量更新
来源：http://hz.shuidangran.top/gtayoeugtk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnqzz.top/gtnpuldypb.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gtpnmtepkm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xingfuxueyuan.xyz/gtlurumicv.html

[Q52] 删除指定行
来源：http://hz.jinghuilouyu.cn/gtpvrrbiju.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtsuaemqth.html

[Q53] 按条件删除
来源：http://hz.snrcjt.cn/gtpycvdgpr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.feifeiyinyue.top/gtyvaktjiy.html

[Q54] 清空表
来源：http://hz.hnxiangtu.top/gtwdbicngx.html

TRUNCATE TABLE logs;
来源：http://hz.zhengqikj.top/gtjlleuqbp.html

[Q55] 排名（并列占位）
来源：http://hz.jyoumei.cn/gttwwkcqrq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinyuanbaomall.cn/gtfxuhesnb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xziqi.cn/gthaabynpx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtfcasvtcv.html

[Q57] 行号
来源：http://hz.redwolf501.top/gthjdygcao.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinghuilouyu.cn/gthykaqfzl.html

[Q58] 累计求和
来源：http://hz.hywenlv.cn/gtsftsezxp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.smart0.xyz/gtqmqngtvw.html

[Q59] 分组内累计
来源：http://hz.jqgfzy.top/gtvcuwrarr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aizwys.cn/gtsbrjdzcf.html

[Q60] 取上一行 / 下一行
来源：http://hz.shanyushiyangkeji.top/gtuzegtgtx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sysykeji.top/gtpmqjmtua.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinqigfzy.top/gtazwnzago.html

[Q61] 移动平均
来源：http://hz.9152youxi.cn/gtenfhneao.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nanxinkj.top/gthsczmldz.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gtazesvvqt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtfyfojkow.html

[Q63] 开启事务
来源：http://hz.nanxuanxn.top/gttnxjvwqh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenlongwang.top/gtmtsmpjjj.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtvyxbleju.html

COMMIT;
来源：http://hz.52xcode.cn/gtuukdfjas.html

[Q65] 回滚事务
来源：http://hz.dianchejie.cn/gtnhslilch.html

ROLLBACK;
来源：http://hz.9152youxi.cn/gtmwsduzvq.html

[Q66] 行锁查询
来源：http://hz.zhongyouzk.top/gtxvijaukh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.smart0.xyz/gtgmwpjpvi.html

[Q67] 设置隔离级别
来源：http://hz.andypj.xyz/gtnjwikzan.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhengqikj.top/gtkuleyyue.html

[Q68] 保存点
来源：http://hz.cucudq.cn/gtudhqtgem.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtakrqnjvq.html

ROLLBACK TO sp1;
来源：http://hz.daria6918.cn/gtekphykpe.html

[Q69] 查看执行计划
来源：http://hz.yongpay.top/gtzwvfrtpr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yangfankeji.com/gtngwuuoyr.html

[Q70] 更新统计信息
来源：http://hz.shzxlz.cn/gtgswebywi.html

ANALYZE TABLE users;
来源：http://hz.nanxuanxn.top/gtptcelvxa.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangtech.top/gtwspurofr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtuurjrwty.html

[Q72] 查看索引
来源：http://hz.9152youxi.cn/gtplnrmfqc.html

SHOW INDEX FROM users;
来源：http://hz.yj202588.top/gtopnaljxa.html

[Q73] 查看表状态
来源：http://hz.hfpthk.cn/gtascwraaf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cheryme.top/gtqjjudzlj.html

[Q74] 强制使用索引
来源：http://hz.nanxinkj.top/gtbgqijbff.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jlsjyb.cn/gtixeohcen.html

[Q75] 日期格式化
来源：http://hz.hfpthk.cn/gtmmjfeqwx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtniqefmqx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shuidangran.top/gtksqmcemd.html

[Q76] 按天统计
来源：http://hz.nanxuanxn.top/gtacuwntmv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxinkj.top/gtwsdzitkw.html

[Q77] 时间加减
来源：http://hz.hnxiangtu.top/gtqqoulpdk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cqqwz.cn/gtazaakuqh.html

[Q78] 当前时间
来源：http://hz.hywenlv.cn/gtmkwpfshj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgufenzy.top/gtiuzbdmee.html

[Q79] 字符串拼接
来源：http://hz.kuanghao11.cn/gttabwtopl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ywan-chungtsiang.top/gtdmgrpimb.html

[Q80] 字符串截取
来源：http://hz.yuanzhike.top/gtnoxncahn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtiqlfvnwa.html

[Q81] 字符串替换
来源：http://hz.guannengcc.top/gtciizdhai.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtbecvzrdt.html

[Q82] 字符长度与字节长度
来源：http://hz.cucudq.cn/gttlavjjnn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hywenlv.cn/gtrwtxwopa.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtbcvqvzyh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cashguo.top/gtuiyohlhk.html

[Q84] 去除首尾空格
来源：http://hz.aibaodan.cn/gtrbmcmavb.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj202588.top/gtejqppkpe.html

[Q85] 数值取整
来源：http://hz.fengsongda.top/gtzazgaemw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhijiandao.cn/gtfnidaomm.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtbdmqcsyg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gogol.net.cn/gtojvwiztt.html

[Q87] JSON 字段做条件
来源：http://hz.mhx1999.top/gtdugqbnwp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258888.top/gtpbmsoyhx.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gtmzpwgbjy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hongshengwenyu.top/gtavzqwjwa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jyoumei.cn/gtpmgudsoj.html

[Q89] 判断表是否存在
来源：http://hz.iojbl.cn/gtgwccpoau.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tian-w.cn/gtnqaykowa.html

[Q90] 生成序号列
来源：http://hz.smart0.xyz/gthexrsmnc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gteytjqukx.html

================================================================================
来源：http://hz.gotoacloud.top/gtvfaqzerl.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtlnutuirg.html

================================================================================
来源：http://hz.zhoulong.xyz/gtacoqleri.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gtgwuiodyk.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtrqxgmwrk.html

set -euo pipefail
来源：http://hz.smart0.xyz/gtqitbfrvi.html

[R02] 变量赋值与使用
来源：http://hz.hnxiangtu.top/gtpzepluew.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtxaciwaxd.html

[R03] 只读变量
来源：http://hz.feifeiyinyue.top/gthekndwhr.html

readonly PI=3.14
来源：http://hz.ywan-chungtsiang.top/gtpeyfniwl.html

[R04] 位置参数
来源：http://hz.hammf.cn/gtdsqnyrvm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtpacubrzg.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtvausdimq.html

name="${1:-default}"
来源：http://hz.jyoumei.cn/gtrcanmdsf.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtnuszesze.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.0kj1m.cn/gtqjoizvum.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtsknkplxn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.dashuyun.cn/gtsvatvznt.html

[R08] 数值比较
来源：http://hz.cheryme.top/gtxhqznozq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.andypj.xyz/gtyxyfbmmt.html

[R09] 字符串比较
来源：http://hz.aizwys.cn/gtcfenqmcb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.316326.xyz/gtrqusdasy.html

[R10] 正则匹配
来源：http://hz.ybcxt.top/gtttcrcblc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.9152youxi.cn/gtiriovdwc.html

[R11] case 多分支
来源：http://hz.sysykeji.top/gtncdjfxei.html

case "$1" in
来源：http://hz.yj202588.top/gtoojipbve.html

start) echo "启动" ;;
来源：http://hz.yj20258.top/gtxvphmxlq.html

stop)  echo "停止" ;;
来源：http://hz.shangyingyoupin.top/gtxorgpqpq.html

*)     echo "未知命令" ;;
来源：http://hz.yangfankeji.com/gtosswcshd.html

esac
来源：http://hz.chenlongwang.top/gtkahcsddj.html

[R12] for 遍历文件
来源：http://hz.andypj.xyz/gtcmjcybco.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cashguo.top/gttaisddfn.html

[R13] for 计数循环
来源：http://hz.yonumen.top/gtbfjbhfku.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hfpthk.cn/gtokjgktep.html

[R14] C 风格 for
来源：http://hz.hysaishi.cn/gtblsrcaov.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dianchejie.cn/gtkxfgpckw.html

[R15] while 逐行读文件
来源：http://hz.chenlongwang.top/gtgxpwrgnu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tianlin.xyz/gtsfgppkbv.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtgyiqmquw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cucudq.cn/gtwuhfgjyz.html

[R17] 数组定义与取值
来源：http://hz.ybcxt.top/gtormcuckg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtkftndoxy.html

[R18] 遍历数组
来源：http://hz.jiagoushi.top/gtvvwirwll.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guowangkeji.top/gtpripquyn.html

[R19] 数组长度
来源：http://hz.dashuyun.cn/gtlaxhkhbf.html

echo "${#arr[@]}"
来源：http://hz.cashguo.top/gtakzdqjlt.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtykiowdly.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jlsjyb.cn/gtbwpqmcyd.html

[R21] 字符串长度
来源：http://hz.gotoacloud.top/gtypnvgpjq.html

echo "${#s}"
来源：http://hz.tian-w.cn/gtpjykeozd.html

[R22] 截取子串
来源：http://hz.wangdashe.top/gtcaagkrns.html

echo "${s:0:5}"
来源：http://hz.jiagoushi.top/gtqhxwznhg.html

[R23] 字符串替换
来源：http://hz.hammf.cn/gtjucinwgw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gotoacloud.top/gtdkugpkod.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtdpqstwsd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhaomingkeji.xyz/gtzebgihat.html

[R25] 去后缀 / 去前缀
来源：http://hz.iojbl.cn/gtrvzonxcy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtjyeytfen.html

[R26] 命令替换
来源：http://hz.daria6918.cn/gthqyzepgk.html

now=$(date +%F); echo "$now"
来源：http://hz.haohaochexian.top/gtuogxknvo.html

[R27] 算术展开
来源：http://hz.yuanzhike.top/gtqwvtwnog.html

echo $((1 + 2 * 3))
来源：http://hz.wangshuangyany.cn/gtamkjftkf.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtvidrfvbs.html

echo "scale=2; 10/3" | bc
来源：http://hz.hnxiangtu.top/gtrbubfluk.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gttttwjqnm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sysykeji.top/gteqipgffv.html

[R30] 函数返回状态码
来源：http://hz.svipenyu.cn/gtzjlnwqyu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.redwolf501.top/gtgxhmpbpe.html

[R31] 局部变量
来源：http://hz.gzhubu.top/gtwzgmtkgu.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangdashe.top/gtmoghnaru.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtpxnyaydb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtequgclty.html

[R33] 捕获错误并提示行号
来源：http://hz.yuanzhike.top/gtnyhmeaod.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258888.top/gtpqnwdbal.html

[R34] 退出时清理
来源：http://hz.ivvv.top/gtyhjxvqhj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gteanbioaq.html

[R35] 后台执行并等待
来源：http://hz.xylfe.cn/gtrlkjvzad.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj202588.top/gtmdpyhjeu.html

[R36] 并发执行多个任务
来源：http://hz.jinqigfzy.top/gtkgwhebqf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jianghu66.top/gtludoumcl.html

[R37] 把输出赋给变量
来源：http://hz.xingfuxueyuan.xyz/gteugtfqsq.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtkxxeisms.html

[R38] 管道串联
来源：http://hz.feifeiyinyue.top/gtoalihwzn.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hfpthk.cn/gtwsxapfxz.html

[R39] 重定向标准输出与错误
来源：http://hz.jinqigufen.top/gttgvulipp.html

cmd > out.log 2>&1
来源：http://hz.ydzc1.top/gtqhbsqiru.html

[R40] 追加写日志
来源：http://hz.0kj1m.cn/gtfwlksuca.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtbzikfhta.html

[R41] 丢弃输出
来源：http://hz.cdnleiting.top/gtcrygbfhg.html

cmd >/dev/null 2>&1
来源：http://hz.yvedp.cn/gtcuuonuko.html

[R42] 输入重定向
来源：http://hz.aibaodan.cn/gtaflsthly.html

wc -l < a.txt
来源：http://hz.kuanghao11.cn/gtgzawmxha.html

[R43] 按名字查找文件
来源：http://hz.redwolf501.top/gthnncuepw.html

find . -name "*.log" -type f
来源：http://hz.ivvv.top/gtckwyzcxa.html

[R44] 按修改时间查找
来源：http://hz.guannengcc.top/gteuljdkor.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtovvrdhai.html

[R45] 批量删除
来源：http://hz.fengsongda.top/gtmsbfobft.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtjxyrkyil.html

[R46] 递归替换文件内容
来源：http://hz.jinyuanbaomall.cn/gtfannzmor.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gtwmtsgjmn.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtlwhdlmrq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtspyovxav.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtdlykqwwx.html

awk '{print $1, $3}' a.txt
来源：http://hz.yanxiufei.cn/gtbvsxrvwq.html

[R49] awk 带条件
来源：http://hz.nwbrower.top/gtczprmmcz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hysaishi.cn/gtdtsigxvl.html

[R50] awk 求和
来源：http://hz.pengpengdd.cyou/gtvyksdwdv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtpttyfbus.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtmeoaxhed.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yongpay.top/gthrcigqhq.html

[R52] 统计行数
来源：http://hz.316326.xyz/gtkehlnwqw.html

wc -l a.txt
来源：http://hz.sufxvd.cn/gtblgeoeoj.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtojqivwaa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.iojbl.cn/gtianjiczu.html

[R54] 比较两个文件
来源：http://hz.birdmap.top/gtlmcpoiml.html

diff a.txt b.txt
来源：http://hz.zhiwuduotai.top/gtfjsewufl.html

[R55] 压缩与解压
来源：http://hz.ybcxt.top/gtfljqwznu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xziqi.cn/gtjemcwdev.html

[R56] 远程拷贝
来源：http://hz.zhoulong.xyz/gtnhqgudok.html

scp file user@host:/path/
来源：http://hz.yj20258.top/gtcnvopebn.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtsccqgnia.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtghrbnmbk.html

[R58] 下载文件
来源：http://hz.hysaishi.cn/gtllcpkdvr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtivpydhpx.html

[R59] 发 POST JSON
来源：http://hz.hysaishi.cn/gtzkapplev.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtfhkioxzj.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtpvfajfov.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cashguo.top/gtswcjeapr.html

[R61] 磁盘占用
来源：http://hz.pycfn.com/gtvpsokcql.html

df -h;  du -sh *
来源：http://hz.zhixingplan.top/gtcmagevic.html

[R62] 找最占空间的文件
来源：http://hz.chenlongwang.top/gtajgizyas.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangtech.top/gtfenmcobp.html

[R63] 内存与进程
来源：http://hz.aibaodan.cn/gtpijeqooa.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtstimheqh.html

[R64] 结束进程
来源：http://hz.sxryk.cn/gtzcybshob.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yueranfly.top/gtnktqiuyl.html

[R65] 查看端口占用
来源：http://hz.jqgufenzy.top/gtqepaecgg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.feifeiyinyue.top/gtmbnczjbi.html

[R66] 定时任务
来源：http://hz.ppjwa.cn/gtthcgsldn.html

crontab -e;  crontab -l
来源：http://hz.feifeiyinyue.top/gtwuumdikd.html

[R67] 生成随机十六进制串
来源：http://hz.hnxiangtu.top/gtiavuptbf.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gtwttuwrcf.html

[R68] 计算文件校验值
来源：http://hz.mhx1999.top/gtafdbbmyc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sweek.top/gtwkhqvutx.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtsnvltxos.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnxiangtu.top/gtigrwvioq.html

[R70] 时间戳与互转
来源：http://hz.smart0.xyz/gtrkdrljto.html

date +%s;  date -d @1700000000
来源：http://hz.shanyushiyangkeji.top/gtaiknbadb.html

[R71] 日期格式化
来源：http://hz.hfpthk.cn/gtsorbixwy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hfpthk.cn/gtekqowwwi.html

[R72] 等待端口就绪
来源：http://hz.hongshengwenyu.top/gtpsnsdrbi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sweek.top/gtzlfvkaup.html

[R73] 分割大日志
来源：http://hz.smart0.xyz/gtqfxfnavu.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtxvaocvla.html

[R74] 批量重命名
来源：http://hz.dianchejie.cn/gtiihultxo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhoulong.xyz/gtivqhjmcx.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtcchxibmq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtbarnemjo.html

[R76] 使用临时文件
来源：http://hz.dashuyun.cn/gtdhaxmbvk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtagudcocb.html

[R77] 读取用户输入
来源：http://hz.dianchejie.cn/gtmantmxfk.html

read -rp "请输入: " ans
来源：http://hz.nanxuanxn.top/gtwzwgxszk.html

[R78] 交互式菜单
来源：http://hz.redwolf501.top/gtwjcygoge.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinghuilouyu.cn/gtnguayfjl.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtbennklua.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gaohongyu789.top/gttjampmvm.html

[R80] 查看脚本执行耗时
来源：http://hz.zhaomingkeji.xyz/gtrovbymdj.html

time ./run.sh
来源：http://hz.zhoulong.xyz/gtvjnfikzf.html

================================================================================
来源：http://hz.kuanghao11.cn/gtaosxziyl.html

S. C / C++ 专题
来源：http://hz.gotoacloud.top/gtuvqeclds.html

================================================================================
来源：http://hz.redwolf501.top/gtbanljuqf.html

[S01] C：Hello World
来源：http://hz.jlsjyb.cn/gtrovnjmfe.html

#include <stdio.h>
来源：http://hz.zdqjudy.top/gtihzwkbkw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hammf.cn/gtgundwapr.html

[S02] C：变量与格式化输出
来源：http://hz.xuanzx.com/gtllfemmny.html

int a = 10; printf("%d\n", a);
来源：http://hz.mhx1999.top/gtxnxcobde.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtywjjljvx.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gtrhgsbcpg.html

[S04] C：字符串复制
来源：http://hz.zhoulong.xyz/gtdadlgzdo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtfedibvqi.html

[S05] C：字符串长度
来源：http://hz.shangyingyoupin.top/gtkarnquzr.html

strlen(s)
来源：http://hz.sufxvd.cn/gtrbsbeoyo.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gtzzaznibt.html

strcmp(a, b) == 0
来源：http://hz.zhaomingkeji.xyz/gtxlugwjbj.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangtech.top/gtaqrnaepf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gaohongyu789.top/gtjuwwrwyi.html

[S08] C：动态内存分配与释放
来源：http://hz.yonumen.top/gtzimvezeb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jianghu66.top/gtndsijuyq.html

[S09] C：结构体定义与初始化
来源：http://hz.gaohongyu789.top/gtrgesvxen.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jyoumei.cn/gtcqcwjyit.html

[S10] C：指针与解引用
来源：http://hz.mhx1999.top/gtrnzlzgsx.html

int *p = &a;  *p = 5;
来源：http://hz.yuxming.cn/gttuczqhnk.html

[S11] C：逐行读文件
来源：http://hz.yongpay.top/gtznnvvynu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gtfkcfiguo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.snrcjt.cn/gtsyrvovwg.html

fclose(f);
来源：http://hz.andypj.xyz/gtdyqfktzh.html

[S12] C：写文件
来源：http://hz.tanke756.top/gtupgbbmub.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gtalmqhgmo.html

[S13] C：宏定义
来源：http://hz.nanxinkj.top/gtheibhqqa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.9152youxi.cn/gttbcokzbq.html

[S14] C：枚举
来源：http://hz.yanxiufei.cn/gtonvjuehb.html


<!-- 参考信息 -->