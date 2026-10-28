代发 wailian999

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtfvfroxle.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tianlin.xyz/gtqdemlpia.html

[Q34] 每组取第一条
来源：http://hz.c1oappe.top/gtmagfswtv.html

SELECT * FROM (
来源：http://hz.gogol.net.cn/gtwstaidrv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtsqsnocvd.html

) t WHERE rn = 1;
来源：http://hz.yuxming.cn/gtoxzxxmed.html

[Q35] 内连接
来源：http://hz.zhijiandao.cn/gtrfummtfn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtrkciovvp.html

[Q36] 左连接
来源：http://hz.ywan-chungtsiang.top/gtrbuwoxpr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtlpbldnml.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gtbgtibzxj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangdashe.top/gthioyfbmt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sxryk.cn/gtgjadhvkg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gtzdporait.html

[Q39] 自连接（查上下级）
来源：http://hz.yueranfly.top/gtfqnbzdqn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnqzz.top/gttzursrbc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.havefunace.top/gtcvlchcmn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gaohongyu789.top/gtsfsqdxyx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pycfn.com/gttnfepraz.html

[Q41] 多表连接
来源：http://hz.yongpay.top/gthmjrlpci.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fengsongda.top/gtqyzzluze.html

JOIN users u ON u.id = o.user_id
来源：http://hz.quarkkingdee.top/gtqgtedxmx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhixingplan.top/gtygpequeb.html

[Q42] 连接条件附加过滤
来源：http://hz.haohaochexian.top/gtfhguhltv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sxryk.cn/gtwhkklged.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aizwys.cn/gtmsimeasy.html

[Q43] 标量子查询
来源：http://hz.xuanzx.com/gtrcohpklt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gthcwtnngy.html

[Q44] IN 子查询
来源：http://hz.yangfankeji.com/gtijhrwpth.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daxiang520.top/gtzimlxarp.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgfzy.top/gtimvmqgcy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtkktcymss.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sufxvd.cn/gtszunigqi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhoulong.xyz/gtyrxxudah.html

[Q47] 与平均值比较
来源：http://hz.ehwqpu.com/gtmaetwvbi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258888.top/gtyzlhhxqt.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangkeji.top/gtlcqmgvpb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.dashuyun.cn/gtwapqjiln.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daxiang520.top/gtmxayzlvc.html

[Q49] 更新单行
来源：http://hz.jinqigufen.top/gtjpybisah.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigfzy.top/gtnjzsetow.html

[Q50] 批量更新
来源：http://hz.jyoumei.cn/gtulykaokl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhaomingkeji.xyz/gtxrpcvvkz.html

[Q51] 用子查询更新
来源：http://hz.zhijiandao.cn/gtvyovhnsd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xingfuxueyuan.xyz/gtsjosfunb.html

[Q52] 删除指定行
来源：http://hz.jlsjyb.cn/gttzsdfzwp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtqyuqbyzc.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gtzivsbuzk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.dianchejie.cn/gthfziomtc.html

[Q54] 清空表
来源：http://hz.svipenyu.cn/gtuduayrwv.html

TRUNCATE TABLE logs;
来源：http://hz.fzhhl.top/gtoqxfitcx.html

[Q55] 排名（并列占位）
来源：http://hz.aizwys.cn/gtatgznmus.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guannengcc.top/gtpgjgfjmz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shuidangran.top/gtxvwtzvhb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yongpay.top/gtufbncczx.html

[Q57] 行号
来源：http://hz.aizwys.cn/gtcfkjwycv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ywan-chungtsiang.top/gthgbyoojd.html

[Q58] 累计求和
来源：http://hz.yj20258888.top/gtapzwfjad.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.52xcode.cn/gterfbwnqd.html

[Q59] 分组内累计
来源：http://hz.316326.xyz/gtujaadxcb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xziqi.cn/gtwkmctupx.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuanzx.com/gtlxwaukpr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hywenlv.cn/gtapyvabkx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zdqjudy.top/gtqhyxjpdm.html

[Q61] 移动平均
来源：http://hz.wangshuangyany.cn/gtggxywcoj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ppjwa.cn/gtgeckjwpn.html

[Q62] 分组占比
来源：http://hz.kuanghao11.cn/gtvkuosryb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtdtapxcsw.html

[Q63] 开启事务
来源：http://hz.yongpay.top/gtcnnuublh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtwbayghzx.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtbodmktpg.html

COMMIT;
来源：http://hz.nanxinkj.top/gtowdxonzi.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtscuxnxru.html

ROLLBACK;
来源：http://hz.redwolf501.top/gtmpacceib.html

[Q66] 行锁查询
来源：http://hz.daria6918.cn/gtcrxrchoo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yonumen.top/gtfuyupxhv.html

[Q67] 设置隔离级别
来源：http://hz.iojbl.cn/gtclwglwwc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hfpthk.cn/gtjtkwvjja.html

[Q68] 保存点
来源：http://hz.shuidangran.top/gtbmxqopgk.html

SAVEPOINT sp1;
来源：http://hz.yuanzhike.top/gthdkgqzdd.html

ROLLBACK TO sp1;
来源：http://hz.cashguo.top/gtdhcswqln.html

[Q69] 查看执行计划
来源：http://hz.zhiwuduotai.top/gtetmsyckb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258.top/gtqrhdywlm.html

[Q70] 更新统计信息
来源：http://hz.aizwys.cn/gtggluajbt.html

ANALYZE TABLE users;
来源：http://hz.jinghuilouyu.cn/gtuudbqpqm.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtrrwgffqh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhijiandao.cn/gtuevovqpv.html

[Q72] 查看索引
来源：http://hz.cashguo.top/gtuewxtliu.html

SHOW INDEX FROM users;
来源：http://hz.fengsongda.top/gtwapawsxt.html

[Q73] 查看表状态
来源：http://hz.yj20258888.top/gtpwvowfhi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gtepfiakfu.html

[Q74] 强制使用索引
来源：http://hz.ehwqpu.com/gtemajtwue.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.bjfxy.top/gtahejuzec.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtmxnihwct.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.vqdsnc.cn/gteyhvvguh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtxpacvtvb.html

[Q76] 按天统计
来源：http://hz.wangdashe.top/gtgamhojyo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sxryk.cn/gtdmsqagpk.html

[Q77] 时间加减
来源：http://hz.dashuyun.cn/gtygtslahw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgfzy.top/gtfialmmju.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtuyqzaijp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258.top/gtnibxtssc.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtjewtvsoz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigufen.top/gtvoxknfwj.html

[Q80] 字符串截取
来源：http://hz.tianlin.xyz/gtplhyzbzz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhoulong.xyz/gtqjchwfba.html

[Q81] 字符串替换
来源：http://hz.yonumen.top/gtvmowuknz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxinkj.top/gtjqkjzmds.html

[Q82] 字符长度与字节长度
来源：http://hz.haohaochexian.top/gtyndvxwzc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangdashe.top/gtonxhueui.html

[Q83] 大小写转换
来源：http://hz.shuidangran.top/gtzosujgnt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgufenzy.top/gtdjdxaxxw.html

[Q84] 去除首尾空格
来源：http://hz.jiagoushi.top/gtejivlzrx.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtvxnmruqt.html

[Q85] 数值取整
来源：http://hz.svipenyu.cn/gtjhlpcflr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhaomingkeji.xyz/gtcnyscdxb.html

[Q86] 读取 JSON 字段
来源：http://hz.hnqzz.top/gtrxlnkzwm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.pycfn.com/gtzjvsvclv.html

[Q87] JSON 字段做条件
来源：http://hz.nwbrower.top/gtdrzjgpej.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yanxiufei.cn/gtaiqtvprk.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhixingplan.top/gtbkeniodu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sweek.top/gtsplqngct.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.mhx1999.top/gtylbqabwp.html

[Q89] 判断表是否存在
来源：http://hz.wangdashe.top/gtebkimhxj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtcztxnmjl.html

[Q90] 生成序号列
来源：http://hz.bjfxy.top/gteyyjtysm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.guowangkeji.top/gtqtykrgiv.html

================================================================================
来源：http://hz.snrcjt.cn/gtvunkjuba.html

R. Bash 专题
来源：http://hz.jlsjyb.cn/gtkbseudwx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzxefoqqa.html

[R01] shebang 与严格模式
来源：http://hz.sweek.top/gthxbyhrcm.html

#!/usr/bin/env bash
来源：http://hz.yanxiufei.cn/gtabpwmkmg.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtfkppcrnr.html

[R02] 变量赋值与使用
来源：http://hz.tian-w.cn/gtthvfokxa.html

name="Tom"; echo "$name"
来源：http://hz.yangfankeji.com/gtuycqvihv.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtoxyfkrhf.html

readonly PI=3.14
来源：http://hz.jinqigfzy.top/gtpnbdehjy.html

[R04] 位置参数
来源：http://hz.sxryk.cn/gteyajgtkt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.meibo888.top/gtxrxxwzdi.html

[R05] 参数默认值
来源：http://hz.yvedp.cn/gtalimkfcg.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtkuhaayfx.html

[R06] 判断命令是否存在
来源：http://hz.ywan-chungtsiang.top/gtrdkvohvp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtuyyrnmko.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gtkdhaesld.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yanxiufei.cn/gtdnroxser.html

[R08] 数值比较
来源：http://hz.9152youxi.cn/gtegnevidt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtguzsikwu.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gtgbpmhraw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jianghu66.top/gtgemfgeen.html

[R10] 正则匹配
来源：http://hz.aizwys.cn/gtwyksagds.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinyuanbaomall.cn/gtfovqsgvd.html

[R11] case 多分支
来源：http://hz.yvedp.cn/gtoufmontv.html

case "$1" in
来源：http://hz.nwbrower.top/gtbaoxecwm.html

start) echo "启动" ;;
来源：http://hz.haohaochexian.top/gtrkbyzryh.html

stop)  echo "停止" ;;
来源：http://hz.daxiang520.top/gtmwqcxyxz.html

*)     echo "未知命令" ;;
来源：http://hz.meibo888.top/gtfkuhutct.html

esac
来源：http://hz.shanyushiyangtech.top/gtloddliqq.html

[R12] for 遍历文件
来源：http://hz.redwolf501.top/gtqrjqbaot.html

for f in *.txt; do echo "$f"; done
来源：http://hz.kuanghao11.cn/gtismjzqiu.html

[R13] for 计数循环
来源：http://hz.tanke756.top/gtrkxnlevg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtwyofrwni.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gtfbxskdpp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtenzgsgww.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gtixchcbae.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ydjk.org.cn/gtlqkawsaz.html

[R16] until 等待条件
来源：http://hz.316326.xyz/gtsryfgiuj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtrmigskjn.html

[R17] 数组定义与取值
来源：http://hz.jqgfzy.top/gtakmbdpkc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gzhubu.top/gtneivhfpg.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gthzrrvpee.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gtetpyuknj.html

[R19] 数组长度
来源：http://hz.ppjwa.cn/gtdswinfuj.html

echo "${#arr[@]}"
来源：http://hz.hnxiangtu.top/gtbuwwcizv.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtzdfzicxb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.andypj.xyz/gtimeobrgh.html

[R21] 字符串长度
来源：http://hz.52xcode.cn/gtoquqpqck.html

echo "${#s}"
来源：http://hz.9152youxi.cn/gtljiogzlo.html

[R22] 截取子串
来源：http://hz.zdqjudy.top/gtjvekfray.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtraentfff.html

[R23] 字符串替换
来源：http://hz.cashguo.top/gturuhvble.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gaohongyu789.top/gtmdxegmqd.html

[R24] 大小写转换
来源：http://hz.xylfe.cn/gtmsirvwng.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigfzy.top/gtgpemwlhk.html

[R25] 去后缀 / 去前缀
来源：http://hz.daxiang520.top/gtfduretdt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yangfankeji.com/gtouufvsqu.html

[R26] 命令替换
来源：http://hz.shanyushiyangtech.top/gtrqtmfdfl.html

now=$(date +%F); echo "$now"
来源：http://hz.jyoumei.cn/gtldxtpywo.html

[R27] 算术展开
来源：http://hz.zhongyouzk.top/gtbzmevrun.html

echo $((1 + 2 * 3))
来源：http://hz.jqgufenzy.top/gtkdplqwei.html

[R28] 浮点运算
来源：http://hz.wangdashe.top/gtulitplog.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtyrmmtomz.html

[R29] 定义函数
来源：http://hz.sweek.top/gtzjdykirz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenlongwang.top/gtpjjscmrr.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtfkdviqzj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fengsongda.top/gtjzngfrbv.html

[R31] 局部变量
来源：http://hz.9152youxi.cn/gtewyohgip.html

f() { local x=1; echo "$x"; }
来源：http://hz.xingfuxueyuan.xyz/gtkwtjgmye.html

[R32] 参数个数校验
来源：http://hz.cqqwz.cn/gtlrhjdsjq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.iojbl.cn/gtxwzakjpe.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtxpcaczye.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtskigbjdh.html

[R34] 退出时清理
来源：http://hz.haohaochexian.top/gtywffsvit.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtgvpeqzzo.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtvbaqwzdl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.quarkkingdee.top/gthwpzmvbt.html

[R36] 并发执行多个任务
来源：http://hz.andypj.xyz/gtndjkpluc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jinyuanbaomall.cn/gtsuniehro.html

[R37] 把输出赋给变量
来源：http://hz.shuidangran.top/gtmtdxjqaz.html

files=$(ls -1)
来源：http://hz.ivvv.top/gtvigvhlng.html

[R38] 管道串联
来源：http://hz.ywan-chungtsiang.top/gttvrnfyti.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtjbvcourj.html

[R39] 重定向标准输出与错误
来源：http://hz.haohaochexian.top/gtkbfimybq.html

cmd > out.log 2>&1
来源：http://hz.redwolf501.top/gtlnvpsjdl.html

[R40] 追加写日志
来源：http://hz.hysaishi.cn/gtheqososf.html

echo "log" >> out.log
来源：http://hz.guowangkeji.top/gtnizvmcvo.html

[R41] 丢弃输出
来源：http://hz.yj20258.top/gtzdfulrrz.html

cmd >/dev/null 2>&1
来源：http://hz.ydzc1.top/gtobuectji.html

[R42] 输入重定向
来源：http://hz.zhengqikj.top/gtwtyfhbqn.html

wc -l < a.txt
来源：http://hz.jlsjyb.cn/gtnanezgjp.html

[R43] 按名字查找文件
来源：http://hz.zhengqikj.top/gtktjewvdr.html

find . -name "*.log" -type f
来源：http://hz.tianlin.xyz/gteohxrujq.html

[R44] 按修改时间查找
来源：http://hz.zhiwuduotai.top/gtaylmjolq.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtuotyvfwk.html

[R45] 批量删除
来源：http://hz.xuetiantiany.cn/gtxyfyxidr.html

find . -name "*.tmp" -delete
来源：http://hz.nwbrower.top/gtnbentunv.html

[R46] 递归替换文件内容
来源：http://hz.nanxuanxn.top/gtcbbjxrdl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pengpengdd.cyou/gtqcyihuoj.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gthmwjlkub.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtnybqehtt.html

[R48] awk 取指定列
来源：http://hz.ivvv.top/gtalcexsjw.html

awk '{print $1, $3}' a.txt
来源：http://hz.shzxlz.cn/gtufkyuiew.html

[R49] awk 带条件
来源：http://hz.sxryk.cn/gtdpvcnpnc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenzaomai.com/gtqraswhqd.html

[R50] awk 求和
来源：http://hz.aibaodan.cn/gtlyfcwfan.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fengsongda.top/gtfjttrwud.html

[R51] 排序去重取前几
来源：http://hz.daria6918.cn/gtbmtevqrx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtyeuwhuui.html

[R52] 统计行数
来源：http://hz.dashuyun.cn/gtaoykefbq.html

wc -l a.txt
来源：http://hz.jianghu66.top/gtqnxugonz.html

[R53] 查看文件头与实时尾
来源：http://hz.mhx1999.top/gtjmokogpb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hongshengwenyu.top/gtfgpexuka.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtmbwqfbbk.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gtkcpovzad.html

[R55] 压缩与解压
来源：http://hz.yj202588.top/gtumyyxzin.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.iojbl.cn/gtxfnchqts.html

[R56] 远程拷贝
来源：http://hz.yj20258.top/gtaazzcdzh.html

scp file user@host:/path/
来源：http://hz.xziqi.cn/gtxxegfbyc.html

[R57] 远程执行命令
来源：http://hz.9152youxi.cn/gtqunjyeug.html

ssh user@host 'uptime'
来源：http://hz.zhaomingkeji.xyz/gtgenqivwc.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gtwlckfvhf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinghuilouyu.cn/gtddviljpb.html

[R59] 发 POST JSON
来源：http://hz.hywenlv.cn/gtogkfurvn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtgeisjdhd.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtkrlsulas.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigfzy.top/gtnngciwgp.html

[R61] 磁盘占用
来源：http://hz.xziqi.cn/gtjujstwzl.html

df -h;  du -sh *
来源：http://hz.dashuyun.cn/gtbaxefeue.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtiwqcachf.html

du -ah . | sort -rh | head -10
来源：http://hz.jiagoushi.top/gtwggdejux.html

[R63] 内存与进程
来源：http://hz.zhoulong.xyz/gtszxaerzk.html

free -h;  ps aux | grep nginx
来源：http://hz.svipenyu.cn/gtngzfhxdd.html

[R64] 结束进程
来源：http://hz.jinqigfzy.top/gtltacynlu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jiagoushi.top/gtlyrmovdk.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gtizpoxqga.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangdashe.top/gttnngfkrg.html

[R66] 定时任务
来源：http://hz.ybcxt.top/gthhkkhoid.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtqmowcvxy.html

[R67] 生成随机十六进制串
来源：http://hz.shzxlz.cn/gtxolrcjnu.html

openssl rand -hex 16
来源：http://hz.ivvv.top/gtbsnhifmy.html

[R68] 计算文件校验值
来源：http://hz.xziqi.cn/gtvabwublj.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangshuangyany.cn/gtqzbwdgtm.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gtizdrogjv.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtofqrmhhi.html

[R70] 时间戳与互转
来源：http://hz.jiagoushi.top/gtkbfilspg.html

date +%s;  date -d @1700000000
来源：http://hz.ivvv.top/gtyrvryuni.html

[R71] 日期格式化
来源：http://hz.jqgufenzy.top/gtehrnygzo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xinyue.icu/gttipxnooi.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtjkdueumo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aibaodan.cn/gtqmbgmbgg.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtmmqpqroo.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtiupbsjri.html

[R74] 批量重命名
来源：http://hz.gaohongyu789.top/gtixvwsjqz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.52xcode.cn/gtysoatpou.html

[R75] 导出环境变量
来源：http://hz.hnqzz.top/gtpyspvfid.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yuanzhike.top/gttiedrcqo.html

[R76] 使用临时文件
来源：http://hz.yj202588.top/gtrfekkfyk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtjpaepkbs.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gtfpalpqni.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtbdkutmlz.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtjkguoyep.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.svipenyu.cn/gtjjbwnfxw.html

[R79] 解析命令行选项
来源：http://hz.iojbl.cn/gtamyiopiv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuanzx.com/gtbvjusqnl.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gtnivayvdk.html

time ./run.sh
来源：http://hz.shzxlz.cn/gtecjafqvg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtrvkevyyf.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtdyaywcsj.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrkqekiom.html

[S01] C：Hello World
来源：http://hz.zhoulong.xyz/gtccqynjzj.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gtisjmbmsd.html


<!-- 参考信息 -->