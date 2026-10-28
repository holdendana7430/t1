代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.9152youxi.cn/gtqjdjfpoa.html

) t WHERE rn = 1;
来源：http://hz.chenjidiqi.icu/gtlfosknar.html

[Q35] 内连接
来源：http://hz.cdnleiting.top/gtlioslpfu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtjdmzvtnx.html

[Q36] 左连接
来源：http://hz.xuanzx.com/gtjiyfwwge.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtnjljxbxw.html

[Q37] 右连接
来源：http://hz.tanke756.top/gtgzoxbiyg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.316326.xyz/gtaphswkaq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhongyouzk.top/gttsfrtsdp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sufxvd.cn/gtzrchefsz.html

[Q39] 自连接（查上下级）
来源：http://hz.yanxiufei.cn/gtqvtqvfkm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dashuyun.cn/gtnrhjibke.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gzhubu.top/gthffnmanb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgufenzy.top/gtgvonstdx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.svipenyu.cn/gtstutxzca.html

[Q41] 多表连接
来源：http://hz.hongshengwenyu.top/gtufiuzvkc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cashguo.top/gtluteyrxj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jlsjyb.cn/gtxwrtpczp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shangyingyoupin.top/gtkwoftuhw.html

[Q42] 连接条件附加过滤
来源：http://hz.kuanghao11.cn/gtmlmjxinp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fengsongda.top/gtowthente.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gtaqiabgeo.html

[Q43] 标量子查询
来源：http://hz.yj202588.top/gtinviesjo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.kuanghao11.cn/gtgejfybkp.html

[Q44] IN 子查询
来源：http://hz.wangshuangyany.cn/gtrmjupsio.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fzhhl.top/gtfucbrbxh.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gtgnstcgvs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtijrpyfhy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.meibo888.top/gtlnwoftwj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtqeimquaf.html

[Q47] 与平均值比较
来源：http://hz.jiagoushi.top/gtiiblpqvo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258.top/gtjkrljtfc.html

[Q48] CTE 公用表表达式
来源：http://hz.quarkkingdee.top/gtypgdzzic.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yvedp.cn/gtmlioivgf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yangfankeji.com/gtxlzmjiib.html

[Q49] 更新单行
来源：http://hz.zdqjudy.top/gtptlwqmta.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtipzokxxo.html

[Q50] 批量更新
来源：http://hz.yuxming.cn/gtfklakdgu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yvedp.cn/gtlnwrmwmf.html

[Q51] 用子查询更新
来源：http://hz.zhoulong.xyz/gtbucbwtsb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtmyglhygr.html

[Q52] 删除指定行
来源：http://hz.daxiang520.top/gtkroewyju.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shzxlz.cn/gtxpahshnr.html

[Q53] 按条件删除
来源：http://hz.jinyuanbaomall.cn/gtnswhyxwv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jianghu66.top/gtsynbsexa.html

[Q54] 清空表
来源：http://hz.cdnleiting.top/gtxtsfabfi.html

TRUNCATE TABLE logs;
来源：http://hz.wangshuangyany.cn/gtdsbyhjur.html

[Q55] 排名（并列占位）
来源：http://hz.daxiang520.top/gtjhsvtwhd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtxtxatlhs.html

[Q56] 密集排名（并列不占位）
来源：http://hz.feifeiyinyue.top/gtuzslurzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtgugrmhlk.html

[Q57] 行号
来源：http://hz.xziqi.cn/gtnlvcmtfd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtknaupdmb.html

[Q58] 累计求和
来源：http://hz.52xcode.cn/gtipitmtbg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sxryk.cn/gtjukdettx.html

[Q59] 分组内累计
来源：http://hz.yj202588.top/gtnrzpctko.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shangyingyoupin.top/gtdwqlicvh.html

[Q60] 取上一行 / 下一行
来源：http://hz.meibo888.top/gtdysbnfib.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yonumen.top/gtkghmtctz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.smart0.xyz/gtrvzzgsrf.html

[Q61] 移动平均
来源：http://hz.aizwys.cn/gtbumozugb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shzxlz.cn/gtznhzelpz.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gtwzdnetam.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtkdodhawg.html

[Q63] 开启事务
来源：http://hz.jianghu66.top/gtvrfpucal.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gtdrrxkzvl.html

[Q64] 提交事务
来源：http://hz.jinqigufen.top/gtwulcaxku.html

COMMIT;
来源：http://hz.yj202588.top/gtvcwcfqpx.html

[Q65] 回滚事务
来源：http://hz.jinqigfzy.top/gtufvqvbak.html

ROLLBACK;
来源：http://hz.ehwqpu.com/gtviiqqmxy.html

[Q66] 行锁查询
来源：http://hz.wangdashe.top/gtqqyedpsp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hywenlv.cn/gtvtdnfqdw.html

[Q67] 设置隔离级别
来源：http://hz.iojbl.cn/gtlrokyuso.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangshuangyany.cn/gtqlvqmvjv.html

[Q68] 保存点
来源：http://hz.sxryk.cn/gtrkzfqvcr.html

SAVEPOINT sp1;
来源：http://hz.zycfv.cn/gtfplmkmfo.html

ROLLBACK TO sp1;
来源：http://hz.xinyue.icu/gtozeisrif.html

[Q69] 查看执行计划
来源：http://hz.cucudq.cn/gtmndoeblv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ydzc1.top/gtaqjthwcg.html

[Q70] 更新统计信息
来源：http://hz.cheryme.top/gtjxsrucgx.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtujptmdgx.html

[Q71] 查看建表语句
来源：http://hz.shuidangran.top/gtwhvvyqbz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gtfrwkmpxn.html

[Q72] 查看索引
来源：http://hz.guowangkeji.top/gtjanglngn.html

SHOW INDEX FROM users;
来源：http://hz.dianchejie.cn/gtaodxicyv.html

[Q73] 查看表状态
来源：http://hz.gotoacloud.top/gtqnzbzgwe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yongpay.top/gtdbmluqgx.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtldwalnpv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtqwyxyymt.html

[Q75] 日期格式化
来源：http://hz.yueranfly.top/gtxpxsbubu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ehwqpu.com/gtzhgtkvjz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxuanxn.top/gthqnhvqxw.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gtoaumrqjp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cashguo.top/gtoxiikxsg.html

[Q77] 时间加减
来源：http://hz.yongpay.top/gtjzlhxzfu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinyuanbaomall.cn/gteyiseaob.html

[Q78] 当前时间
来源：http://hz.zycfv.cn/gtsciomira.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xingfuxueyuan.xyz/gtvcoepxww.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtoeahxpza.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.svipenyu.cn/gtyngbajfr.html

[Q80] 字符串截取
来源：http://hz.yanxiufei.cn/gtpkkpwsom.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtbyklvpkv.html

[Q81] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtdmksdiek.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtarvuxpbx.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtrntmarxl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtgvnhygvk.html

[Q83] 大小写转换
来源：http://hz.nanxinkj.top/gtpjqtxnka.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aibaodan.cn/gtivsedego.html

[Q84] 去除首尾空格
来源：http://hz.vqdsnc.cn/gtpeealikm.html

SELECT TRIM(name) FROM users;
来源：http://hz.aizwys.cn/gtotfqmdbl.html

[Q85] 数值取整
来源：http://hz.hywenlv.cn/gtzrcgwsef.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cdnleiting.top/gtbybpiwbo.html

[Q86] 读取 JSON 字段
来源：http://hz.yueranfly.top/gtklctodem.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hnxiangtu.top/gttbgbtbvm.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtcrkyktyh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hongshengwenyu.top/gtcrqcnbfl.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhixingplan.top/gthcozbnjp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gtgpdmvzun.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.mhx1999.top/gtxyzunlfb.html

[Q89] 判断表是否存在
来源：http://hz.gogol.net.cn/gtsxtfjddg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.c1oappe.top/gthpyxxitl.html

[Q90] 生成序号列
来源：http://hz.ydjk.org.cn/gtsrxhumgz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cucudq.cn/gterozykfk.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlkukugrs.html

R. Bash 专题
来源：http://hz.jyoumei.cn/gtvbwdenif.html

================================================================================
来源：http://hz.guowangkeji.top/gtscsdtusm.html

[R01] shebang 与严格模式
来源：http://hz.jlsjyb.cn/gtvwxfdhcp.html

#!/usr/bin/env bash
来源：http://hz.yvedp.cn/gtlmvdtnrb.html

set -euo pipefail
来源：http://hz.shuidangran.top/gtnwnrirpb.html

[R02] 变量赋值与使用
来源：http://hz.wangdashe.top/gtyhiveamh.html

name="Tom"; echo "$name"
来源：http://hz.nwbrower.top/gtyhwfdwsy.html

[R03] 只读变量
来源：http://hz.jqgufenzy.top/gtgguwusrj.html

readonly PI=3.14
来源：http://hz.pycfn.com/gtidihhoft.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtelhhvxvz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj202588.top/gtumurjnqe.html

[R05] 参数默认值
来源：http://hz.tian-w.cn/gtqaqhbtyk.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtsmejoadv.html

[R06] 判断命令是否存在
来源：http://hz.xylfe.cn/gtsqmgropu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guowangkeji.top/gtoydbnvyh.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtarbhwsnv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtsavlibxy.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gtwnacdaqv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.bjfxy.top/gtabpawypz.html

[R09] 字符串比较
来源：http://hz.xuetiantiany.cn/gthjgdfuhe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.vqdsnc.cn/gtaagbyxbh.html

[R10] 正则匹配
来源：http://hz.ywan-chungtsiang.top/gtndpaxbal.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yuxming.cn/gtydomgtcd.html

[R11] case 多分支
来源：http://hz.gzhubu.top/gtecerlqam.html

case "$1" in
来源：http://hz.wangdashe.top/gtxpfzoxay.html

start) echo "启动" ;;
来源：http://hz.bjfxy.top/gthdktczfm.html

stop)  echo "停止" ;;
来源：http://hz.sysykeji.top/gteyaukrvv.html

*)     echo "未知命令" ;;
来源：http://hz.meibo888.top/gtdtthpqmd.html

esac
来源：http://hz.dianchejie.cn/gtaxvvjmqq.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gthtrtvkpy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xylfe.cn/gtxleyaacm.html

[R13] for 计数循环
来源：http://hz.daria6918.cn/gtjndszvyg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.0kj1m.cn/gtjtjbqygr.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gtrumrtsfy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daria6918.cn/gtejrtuedp.html

[R15] while 逐行读文件
来源：http://hz.daxiang520.top/gtemzaijot.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhoulong.xyz/gtnqjidmyi.html

[R16] until 等待条件
来源：http://hz.yanxiufei.cn/gtmhvszfdi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tianlin.xyz/gthdfxycdd.html

[R17] 数组定义与取值
来源：http://hz.jinqigfzy.top/gtpfyvtlux.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtymqldezn.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtxwharzdi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangdashe.top/gtzgpqtoge.html

[R19] 数组长度
来源：http://hz.nanxuanxn.top/gtblyhwrhz.html

echo "${#arr[@]}"
来源：http://hz.fzhhl.top/gtxhffffta.html

[R20] 关联数组（字典）
来源：http://hz.aizwys.cn/gtxgmiabzv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hywenlv.cn/gtssimagld.html

[R21] 字符串长度
来源：http://hz.hnqzz.top/gtioktygkm.html

echo "${#s}"
来源：http://hz.fzhhl.top/gtvlcvrzvc.html

[R22] 截取子串
来源：http://hz.sufxvd.cn/gtludupuhx.html

echo "${s:0:5}"
来源：http://hz.cucudq.cn/gtmixpgitk.html

[R23] 字符串替换
来源：http://hz.guowangkeji.top/gtuourrafw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.andypj.xyz/gtcyevjvws.html

[R24] 大小写转换
来源：http://hz.hammf.cn/gtlefzkzcv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gtylnfdwyf.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtyzbinhzq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ehwqpu.com/gtdxbvxjah.html

[R26] 命令替换
来源：http://hz.zhoulong.xyz/gtibhiyxjt.html

now=$(date +%F); echo "$now"
来源：http://hz.jiagoushi.top/gtsesnhtvi.html

[R27] 算术展开
来源：http://hz.jinqigufen.top/gtjwvzfobd.html

echo $((1 + 2 * 3))
来源：http://hz.tianlin.xyz/gtjatjqirn.html

[R28] 浮点运算
来源：http://hz.jinqigfzy.top/gtbunlvigg.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxinkj.top/gtiydvgbnk.html

[R29] 定义函数
来源：http://hz.yj20258888.top/gtepxoizwd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangdashe.top/gtdafslaoj.html

[R30] 函数返回状态码
来源：http://hz.daria6918.cn/gtxxrqezpw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtdkwboqeb.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtqnwhwrbp.html

f() { local x=1; echo "$x"; }
来源：http://hz.sysykeji.top/gtdaktagjk.html

[R32] 参数个数校验
来源：http://hz.guannengcc.top/gtzhzckhgy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gtkdgsamtv.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtwrybozom.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zdqjudy.top/gtvlfsbfru.html

[R34] 退出时清理
来源：http://hz.gzhubu.top/gtwkavbmmn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtnkdvkuco.html

[R35] 后台执行并等待
来源：http://hz.gogol.net.cn/gtoycgxpjh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gtdirlnmil.html

[R36] 并发执行多个任务
来源：http://hz.hnxiangtu.top/gtuvrmhryq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258.top/gtgvpaowhf.html

[R37] 把输出赋给变量
来源：http://hz.gogol.net.cn/gtcqhokifr.html

files=$(ls -1)
来源：http://hz.jinghuilouyu.cn/gtwrjgtlbp.html

[R38] 管道串联
来源：http://hz.chenjidiqi.icu/gtwrcpsanq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtbejuvlim.html

[R39] 重定向标准输出与错误
来源：http://hz.yuanzhike.top/gttbivtdum.html

cmd > out.log 2>&1
来源：http://hz.0kj1m.cn/gtxqhhsilr.html

[R40] 追加写日志
来源：http://hz.hnqzz.top/gtybdtdxxf.html

echo "log" >> out.log
来源：http://hz.ivvv.top/gtcwlrdkeq.html

[R41] 丢弃输出
来源：http://hz.jlsjyb.cn/gtwtxijgnl.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtzlnetzxz.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gtwimoxira.html

wc -l < a.txt
来源：http://hz.jinghuilouyu.cn/gtxxppjulu.html

[R43] 按名字查找文件
来源：http://hz.cheryme.top/gtcmtpgwlq.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtabxutkei.html

[R44] 按修改时间查找
来源：http://hz.zhixingplan.top/gtgrheacbg.html

find . -mtime -7 -type f
来源：http://hz.yj20258888.top/gtkyyfcjpf.html

[R45] 批量删除
来源：http://hz.zhixingplan.top/gtprhctedj.html

find . -name "*.tmp" -delete
来源：http://hz.shangyingyoupin.top/gtsnkoyjkn.html

[R46] 递归替换文件内容
来源：http://hz.zhijiandao.cn/gtgkjecjmd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dianchejie.cn/gttsvoahya.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gthbgutnfy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtufjpooiq.html

[R48] awk 取指定列
来源：http://hz.bjfxy.top/gtxavxlnxp.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtdhelwqxt.html

[R49] awk 带条件
来源：http://hz.yongpay.top/gtfnvordap.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.316326.xyz/gtjcasyryl.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtigiwulal.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.mhx1999.top/gtibqgczlh.html

[R51] 排序去重取前几
来源：http://hz.hammf.cn/gtwuzijaxo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgufenzy.top/gtlywjcohb.html

[R52] 统计行数
来源：http://hz.cheryme.top/gtxtkrlocc.html

wc -l a.txt
来源：http://hz.jinqigufen.top/gtmrpcldfq.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gttozmqalr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gthdfkwtan.html

[R54] 比较两个文件
来源：http://hz.yangfankeji.com/gttjkcfzhy.html

diff a.txt b.txt
来源：http://hz.tanke756.top/gticvvgmvr.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtzollixze.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtcoehabez.html

[R56] 远程拷贝
来源：http://hz.9152youxi.cn/gtatxgesri.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtrruospvo.html

[R57] 远程执行命令
来源：http://hz.sysykeji.top/gtfrbcktzk.html

ssh user@host 'uptime'
来源：http://hz.zhongyouzk.top/gtrjnugjiu.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtfuxoudiz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258888.top/gtynmxybcu.html

[R59] 发 POST JSON
来源：http://hz.jinqigfzy.top/gtcvnpjjjd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtxjpwxrkd.html

[R60] 只看 HTTP 状态码
来源：http://hz.dashuyun.cn/gtcrwdalfh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gtnqfbglph.html

[R61] 磁盘占用
来源：http://hz.nanxuanxn.top/gtfzesjzxt.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtrcffufix.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtjbtclvjk.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtmctjdnmj.html

[R63] 内存与进程
来源：http://hz.fzhhl.top/gtoaxqbczv.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtjgayvfgb.html

[R64] 结束进程
来源：http://hz.zhoulong.xyz/gtixuzthuw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aizwys.cn/gtjznbbqrd.html

[R65] 查看端口占用
来源：http://hz.yj20258888.top/gtzyhrjowm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtkfjklora.html

[R66] 定时任务
来源：http://hz.zhengqikj.top/gtkkaljwnt.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gtvmqkaiac.html

[R67] 生成随机十六进制串
来源：http://hz.9152youxi.cn/gtlwglmzdt.html

openssl rand -hex 16
来源：http://hz.haohaochexian.top/gtzkepykof.html

[R68] 计算文件校验值
来源：http://hz.hongshengwenyu.top/gttkeyxufy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.316326.xyz/gtnfunpddr.html

[R69] 生成随机密码
来源：http://hz.daxiang520.top/gtybtucysx.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtctkrrshe.html

[R70] 时间戳与互转
来源：http://hz.vqdsnc.cn/gtaoxvvgfz.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtgplkqmuj.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gtmwktracp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydzc1.top/gtwcejqhov.html

[R72] 等待端口就绪
来源：http://hz.yvedp.cn/gtvpnutlrz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtakxkavhw.html

[R73] 分割大日志
来源：http://hz.yueranfly.top/gtgfcllcyw.html

split -l 1000 big.log part_
来源：http://hz.xuanzx.com/gtylvxnnlh.html

[R74] 批量重命名
来源：http://hz.ydjk.org.cn/gthoykgqjj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ppjwa.cn/gtmyvuxaka.html

[R75] 导出环境变量
来源：http://hz.pengpengdd.cyou/gtkduiotrt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.bjfxy.top/gttksiuzfp.html

[R76] 使用临时文件
来源：http://hz.smart0.xyz/gtlszanqlx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gthczpoqfw.html

[R77] 读取用户输入
来源：http://hz.jyoumei.cn/gtxoxxawty.html

read -rp "请输入: " ans
来源：http://hz.aizwys.cn/gtdvizjuxd.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtykykwuko.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jyoumei.cn/gtqqqohuru.html

[R79] 解析命令行选项
来源：http://hz.gaohongyu789.top/gtbcqnikaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtdmafhvhg.html

[R80] 查看脚本执行耗时
来源：http://hz.xuanzx.com/gttauiwrjd.html

time ./run.sh
来源：http://hz.52xcode.cn/gtgkhsxvfm.html

================================================================================
来源：http://hz.aizwys.cn/gthnbzbsep.html

S. C / C++ 专题
来源：http://hz.sysykeji.top/gttdqahzen.html

================================================================================
来源：http://hz.cheryme.top/gtbagbzhij.html

[S01] C：Hello World
来源：http://hz.hysaishi.cn/gtiuzwnspb.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gttwpgcabw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gthsjqvtiu.html

[S02] C：变量与格式化输出
来源：http://hz.vqdsnc.cn/gtzebfvamm.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gtnjhotiop.html

[S03] C：读入整数
来源：http://hz.zhongyouzk.top/gtmgicyuzj.html


<!-- 参考信息 -->