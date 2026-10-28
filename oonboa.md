代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gtsvgzhiqm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.gogol.net.cn/gtbijbmuyr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuanzx.com/gtbirkmmxm.html

[Q41] 多表连接
来源：http://hz.sufxvd.cn/gtpyqlwudk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtzrwgtbmk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigufen.top/gtwqbblllq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258.top/gtcqbwioko.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgufenzy.top/gtsmcwgpjr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shzxlz.cn/gtvgblpvym.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtrkyduaet.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gtshppuggz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yangfankeji.com/gtkxgzbhbi.html

[Q44] IN 子查询
来源：http://hz.chenjidiqi.icu/gtzclouyoq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.redwolf501.top/gtmwyzgzqa.html

[Q45] EXISTS 判断存在
来源：http://hz.yj202588.top/gtbiqelzbx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtaftksqkt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dianchejie.cn/gtzsbqmhsr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtzrbzxbep.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtyfpohyxr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.wangshuangyany.cn/gtgdjgnftp.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtmjkvizsk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtuoeecnew.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnxiangtu.top/gtveuhmaro.html

[Q49] 更新单行
来源：http://hz.0kj1m.cn/gtnjnfkdit.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtouqzkzal.html

[Q50] 批量更新
来源：http://hz.ydjk.org.cn/gtvpiezzax.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ydzc1.top/gtezdmmhov.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtwupczrzu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pengpengdd.cyou/gtnxrduzre.html

[Q52] 删除指定行
来源：http://hz.yueranfly.top/gtzgeniqdr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dianchejie.cn/gtmjvjkjip.html

[Q53] 按条件删除
来源：http://hz.chenlongwang.top/gtvhtypnwb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xinyue.icu/gtrtwartew.html

[Q54] 清空表
来源：http://hz.zycfv.cn/gtgrzwyjzt.html

TRUNCATE TABLE logs;
来源：http://hz.svipenyu.cn/gtklougmgv.html

[Q55] 排名（并列占位）
来源：http://hz.birdmap.top/gtjkhztycv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenlongwang.top/gtfcusprcq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydzc1.top/gtqtgfotwb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtgptcaixa.html

[Q57] 行号
来源：http://hz.shuidangran.top/gtxljvmfmz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtcnufzqnc.html

[Q58] 累计求和
来源：http://hz.bjfxy.top/gtrfksucao.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hysaishi.cn/gtervznxjv.html

[Q59] 分组内累计
来源：http://hz.guannengcc.top/gtwarcbrmw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.0kj1m.cn/gtakfwrfhc.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gttshfxjdp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gzhubu.top/gtcfgnutjq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ppjwa.cn/gtjtcbruik.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtktvujlol.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.c1oappe.top/gtgaoohciz.html

[Q62] 分组占比
来源：http://hz.zdqjudy.top/gtxkhxxxmn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuanzhike.top/gtuaqbuump.html

[Q63] 开启事务
来源：http://hz.hnqzz.top/gtrktxmrsf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xinyue.icu/gttqgyecas.html

[Q64] 提交事务
来源：http://hz.xuetiantiany.cn/gtcytdaman.html

COMMIT;
来源：http://hz.zhengqikj.top/gtlzudgmqg.html

[Q65] 回滚事务
来源：http://hz.dashuyun.cn/gtwwtafzgq.html

ROLLBACK;
来源：http://hz.svipenyu.cn/gtdpjtdghr.html

[Q66] 行锁查询
来源：http://hz.guannengcc.top/gtqiotieba.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zdqjudy.top/gtmkzhnhbd.html

[Q67] 设置隔离级别
来源：http://hz.vqdsnc.cn/gtxwgzrogg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.mhx1999.top/gtiavmgxfp.html

[Q68] 保存点
来源：http://hz.tian-w.cn/gttgdodyol.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtqdzshboc.html

ROLLBACK TO sp1;
来源：http://hz.cucudq.cn/gteatsyeqv.html

[Q69] 查看执行计划
来源：http://hz.hfpthk.cn/gthoseiqof.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yanxiufei.cn/gtomwzrhld.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtpqwiqbbj.html

ANALYZE TABLE users;
来源：http://hz.9152youxi.cn/gtntzrjfis.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtwniwamtw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhengqikj.top/gtcgimdzaf.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gtiadnsoja.html

SHOW INDEX FROM users;
来源：http://hz.zdqjudy.top/gtsbpcicoq.html

[Q73] 查看表状态
来源：http://hz.mhx1999.top/gtttuceggi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.feifeiyinyue.top/gtojisyfcf.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtfgriqcic.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tianlin.xyz/gtxupwtupb.html

[Q75] 日期格式化
来源：http://hz.shangyingyoupin.top/gtsxztdgrs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gaohongyu789.top/gtwpkxpelk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jianghu66.top/gtzpqbmjor.html

[Q76] 按天统计
来源：http://hz.zhengqikj.top/gtopsdyrtk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhengqikj.top/gtbfdaqdgk.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtusmhjfcu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xingfuxueyuan.xyz/gtokkcctdu.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtnuskscvt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aizwys.cn/gtwrubsocy.html

[Q79] 字符串拼接
来源：http://hz.gogol.net.cn/gtpoocibkf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.feifeiyinyue.top/gtisdwxiav.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gtderxhyum.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtrpbosgun.html

[Q81] 字符串替换
来源：http://hz.yuanzhike.top/gtzdgjbxlb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gotoacloud.top/gtyzuclssy.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtnbppyysp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gthhxpcecz.html

[Q83] 大小写转换
来源：http://hz.havefunace.top/gtrukeobys.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuxming.cn/gtveasevav.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtszfuyfll.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuxming.cn/gtljtthcvp.html

[Q85] 数值取整
来源：http://hz.jianghu66.top/gtzpjsxfcv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gzhubu.top/gtqylajynr.html

[Q86] 读取 JSON 字段
来源：http://hz.feifeiyinyue.top/gtbckpwrlf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhaomingkeji.xyz/gtbqulmcba.html

[Q87] JSON 字段做条件
来源：http://hz.hammf.cn/gtcssusvyi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.kuanghao11.cn/gtvniodknj.html

[Q88] 行转列（条件聚合）
来源：http://hz.ivvv.top/gttltymkou.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.bjfxy.top/gtaqbhzawn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtimbtcrxd.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtmczhgodo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xuetiantiany.cn/gtqekjspam.html

[Q90] 生成序号列
来源：http://hz.cheryme.top/gtnlfmjdqf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtjjbkobiu.html

================================================================================
来源：http://hz.jyoumei.cn/gtabapoceq.html

R. Bash 专题
来源：http://hz.hfpthk.cn/gtcbtwlroj.html

================================================================================
来源：http://hz.nwbrower.top/gtbduwwpxi.html

[R01] shebang 与严格模式
来源：http://hz.quarkkingdee.top/gtcmshnvgw.html

#!/usr/bin/env bash
来源：http://hz.hammf.cn/gtonefnqpg.html

set -euo pipefail
来源：http://hz.0kj1m.cn/gtqwevlbnt.html

[R02] 变量赋值与使用
来源：http://hz.xuanzx.com/gtviptxlai.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangtech.top/gtrdjwpzkh.html

[R03] 只读变量
来源：http://hz.xylfe.cn/gtrrlkcalu.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gtafaxxfii.html

[R04] 位置参数
来源：http://hz.cashguo.top/gtjrtxhgkd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhengqikj.top/gtarlacbic.html

[R05] 参数默认值
来源：http://hz.mhx1999.top/gtprixgitc.html

name="${1:-default}"
来源：http://hz.pycfn.com/gtdpnbvfai.html

[R06] 判断命令是否存在
来源：http://hz.andypj.xyz/gtoycvffof.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuanzx.com/gtilozcptz.html

[R07] if 判断文件
来源：http://hz.snrcjt.cn/gtyjssoebi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jlsjyb.cn/gtzoymycoe.html

[R08] 数值比较
来源：http://hz.cucudq.cn/gtfxnlcbnh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sufxvd.cn/gthvbqjses.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gthqhgfrtg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aibaodan.cn/gtnvxivpkg.html

[R10] 正则匹配
来源：http://hz.fzhhl.top/gtjrnwvlzd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gtsfdotidu.html

[R11] case 多分支
来源：http://hz.zhongyouzk.top/gtyyxafecu.html

case "$1" in
来源：http://hz.yj20258.top/gtgqwgtfnx.html

start) echo "启动" ;;
来源：http://hz.cashguo.top/gtlvjtwheb.html

stop)  echo "停止" ;;
来源：http://hz.tian-w.cn/gtlzmeenuh.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gttbzmezvn.html

esac
来源：http://hz.nanxinkj.top/gtgtecayrt.html

[R12] for 遍历文件
来源：http://hz.meibo888.top/gtlamiakqq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cucudq.cn/gttqybzoxr.html

[R13] for 计数循环
来源：http://hz.andypj.xyz/gtlztwqfat.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhiwuduotai.top/gtlnuykobz.html

[R14] C 风格 for
来源：http://hz.hfpthk.cn/gtnomspepm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gttlomummt.html

[R15] while 逐行读文件
来源：http://hz.ydzc1.top/gtiribcrtp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuanzhike.top/gtywozbace.html

[R16] until 等待条件
来源：http://hz.nwbrower.top/gtzfajxmgd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cqqwz.cn/gthtgvswab.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtidtjdytz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shanyushiyangtech.top/gtnxbkmcib.html

[R18] 遍历数组
来源：http://hz.cucudq.cn/gtbvfrxvmd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtipkimrce.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtqlbutuni.html

echo "${#arr[@]}"
来源：http://hz.daxiang520.top/gtjbwhmtuq.html

[R20] 关联数组（字典）
来源：http://hz.ywan-chungtsiang.top/gtzrpmwiah.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtxcrlbvvs.html

[R21] 字符串长度
来源：http://hz.shanyushiyangtech.top/gtqwhilgix.html

echo "${#s}"
来源：http://hz.hammf.cn/gtzplvnqkw.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtljwumetu.html

echo "${s:0:5}"
来源：http://hz.yonumen.top/gtgmzprfzi.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gtjhfbjuwz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtjqsyijfe.html

[R24] 大小写转换
来源：http://hz.xylfe.cn/gtstrwxmkh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtawrhvepo.html

[R25] 去后缀 / 去前缀
来源：http://hz.jyoumei.cn/gtriumnhcx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtqygwdlxt.html

[R26] 命令替换
来源：http://hz.zhiwuduotai.top/gtqmyxsqrn.html

now=$(date +%F); echo "$now"
来源：http://hz.shzxlz.cn/gtgzqnpjhf.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gtjjtoiwgh.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gtrsowugrl.html

[R28] 浮点运算
来源：http://hz.ppjwa.cn/gtmfrkeodn.html

echo "scale=2; 10/3" | bc
来源：http://hz.ehwqpu.com/gtcczjfspu.html

[R29] 定义函数
来源：http://hz.jyoumei.cn/gtetjpyauz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258.top/gtdgmhxgtg.html

[R30] 函数返回状态码
来源：http://hz.yj20258.top/gttnhpqorh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aizwys.cn/gtwbodgasf.html

[R31] 局部变量
来源：http://hz.feifeiyinyue.top/gtrlfbmidz.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangdashe.top/gtorvlwhiq.html

[R32] 参数个数校验
来源：http://hz.yanxiufei.cn/gtncnrlbif.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhijiandao.cn/gtnxvhthrd.html

[R33] 捕获错误并提示行号
来源：http://hz.yj20258888.top/gtaesukydp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gtnvviksjr.html

[R34] 退出时清理
来源：http://hz.xylfe.cn/gthtvtpypz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtdkpnnupo.html

[R35] 后台执行并等待
来源：http://hz.jinqigufen.top/gtlhvzjrun.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.fzhhl.top/gtswgfhpql.html

[R36] 并发执行多个任务
来源：http://hz.pycfn.com/gtbneqwrnx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.quarkkingdee.top/gtpcpczala.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtlgrcfqpx.html

files=$(ls -1)
来源：http://hz.hnqzz.top/gtjjaurbmy.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtqwfquqjc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.svipenyu.cn/gtymgbcian.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gthjriuizh.html

cmd > out.log 2>&1
来源：http://hz.vqdsnc.cn/gtfyrprshw.html

[R40] 追加写日志
来源：http://hz.jinqigufen.top/gtppqtsmgn.html

echo "log" >> out.log
来源：http://hz.shuidangran.top/gtweyopvbh.html

[R41] 丢弃输出
来源：http://hz.jyoumei.cn/gtwwvtskxi.html

cmd >/dev/null 2>&1
来源：http://hz.yuanzhike.top/gtvnoyahot.html

[R42] 输入重定向
来源：http://hz.ehwqpu.com/gtrmouvgqw.html

wc -l < a.txt
来源：http://hz.gaohongyu789.top/gtfqrdhpla.html

[R43] 按名字查找文件
来源：http://hz.cashguo.top/gtxqsldnky.html

find . -name "*.log" -type f
来源：http://hz.xuetiantiany.cn/gtpqkllywr.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtpvgpfsud.html

find . -mtime -7 -type f
来源：http://hz.smart0.xyz/gtifunqzfe.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtnmlmlrjm.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gtjmzymjvn.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gtkqlizkml.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gtdgfscpuy.html

[R47] sed 单行替换
来源：http://hz.jinyuanbaomall.cn/gtorlpiler.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.smart0.xyz/gtefoegbbg.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtbcurgubk.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gtgpjbumxs.html

[R49] awk 带条件
来源：http://hz.ydjk.org.cn/gtvmvgnecf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tianlin.xyz/gtggezcupe.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtbnipegzn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtmbyyywjh.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gtagskznuz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhengqikj.top/gtvgkopklm.html

[R52] 统计行数
来源：http://hz.tanke756.top/gtuyogcdcg.html

wc -l a.txt
来源：http://hz.hnqzz.top/gtntqsefqs.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258888.top/gtrembkktz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shangyingyoupin.top/gtguqgywkz.html

[R54] 比较两个文件
来源：http://hz.redwolf501.top/gtuutglqaj.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtyrivsivi.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtivimjezj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhijiandao.cn/gtdsmslrei.html

[R56] 远程拷贝
来源：http://hz.hongshengwenyu.top/gtxvphovhg.html

scp file user@host:/path/
来源：http://hz.316326.xyz/gthismlbia.html

[R57] 远程执行命令
来源：http://hz.yj20258.top/gthjxmgrlw.html

ssh user@host 'uptime'
来源：http://hz.cashguo.top/gtvptnsijt.html

[R58] 下载文件
来源：http://hz.aibaodan.cn/gtoxisqcjm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtfqftuqsj.html

[R59] 发 POST JSON
来源：http://hz.shzxlz.cn/gtaqkmfbou.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhengqikj.top/gtjmyrbnyv.html

[R60] 只看 HTTP 状态码
来源：http://hz.aizwys.cn/gtvgjdutgu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtrsnpoahd.html

[R61] 磁盘占用
来源：http://hz.jianghu66.top/gtgzxujjzo.html

df -h;  du -sh *
来源：http://hz.xziqi.cn/gtlnblkewj.html

[R62] 找最占空间的文件
来源：http://hz.kuanghao11.cn/gtfcgwzqnb.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtcxvczehu.html

[R63] 内存与进程
来源：http://hz.tanke756.top/gtdcpybhyp.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtbgqdcxfa.html

[R64] 结束进程
来源：http://hz.xziqi.cn/gtydjawneu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tian-w.cn/gtqlwjcouw.html

[R65] 查看端口占用
来源：http://hz.fengsongda.top/gthysppfaq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cdnleiting.top/gtrxorbgzu.html

[R66] 定时任务
来源：http://hz.svipenyu.cn/gtihmnfdnj.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gtcuhsekpx.html

[R67] 生成随机十六进制串
来源：http://hz.yanxiufei.cn/gtdglldfvk.html

openssl rand -hex 16
来源：http://hz.ydjk.org.cn/gtwyuybpym.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gthkqzibwt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtmzclllis.html

[R69] 生成随机密码
来源：http://hz.mhx1999.top/gtzkpzxpgr.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhongyouzk.top/gtxrsacrhw.html

[R70] 时间戳与互转
来源：http://hz.guowangkeji.top/gtibfarzdk.html

date +%s;  date -d @1700000000
来源：http://hz.ybcxt.top/gtrygzbjog.html

[R71] 日期格式化
来源：http://hz.quarkkingdee.top/gteqqcqdpx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj20258.top/gtzdhbkqsa.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtgxmlnnha.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtlrazgwgf.html

[R73] 分割大日志
来源：http://hz.meibo888.top/gtfrpqchxl.html

split -l 1000 big.log part_
来源：http://hz.xuetiantiany.cn/gtnfgldwfm.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtkoixpems.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jlsjyb.cn/gtzvarlzxw.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gtflvsosth.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtcdbkaxlk.html

[R76] 使用临时文件
来源：http://hz.gogol.net.cn/gtgumekten.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtcrnwwcrq.html

[R77] 读取用户输入
来源：http://hz.yj20258888.top/gtdxuioqlf.html

read -rp "请输入: " ans
来源：http://hz.cdnleiting.top/gtzchkdjzz.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtgchqbjig.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtiegmxgvq.html

[R79] 解析命令行选项
来源：http://hz.smart0.xyz/gtfxbahcrf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ehwqpu.com/gtxvhwbjzg.html

[R80] 查看脚本执行耗时
来源：http://hz.yanxiufei.cn/gtjmxaxsed.html

time ./run.sh
来源：http://hz.hammf.cn/gtrrhpizfv.html

================================================================================
来源：http://hz.gzhubu.top/gtpwrvloqo.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtmcudwpgy.html

================================================================================
来源：http://hz.shuidangran.top/gtmuguozxu.html

[S01] C：Hello World
来源：http://hz.gotoacloud.top/gtdgjgeuvp.html

#include <stdio.h>
来源：http://hz.hongshengwenyu.top/gtzxwebfpk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daria6918.cn/gtriorqixv.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtbxedtrnq.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtjadojcph.html

[S03] C：读入整数
来源：http://hz.jinqigufen.top/gtcuztqswu.html

int x; scanf("%d", &x);
来源：http://hz.hywenlv.cn/gthqcibumo.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtxnljpcek.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pengpengdd.cyou/gtvldrzbvo.html

[S05] C：字符串长度
来源：http://hz.chenzaomai.com/gtwkrkzenz.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtymjadtsu.html

[S06] C：字符串比较
来源：http://hz.zhijiandao.cn/gtjwjlaeqt.html

strcmp(a, b) == 0
来源：http://hz.pengpengdd.cyou/gthfvslvin.html

[S07] C：数组遍历求和
来源：http://hz.jinqigfzy.top/gtlibhecyi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.meibo888.top/gtjovelbrg.html

[S08] C：动态内存分配与释放
来源：http://hz.tianlin.xyz/gttictafhs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtwfaasyjg.html

[S09] C：结构体定义与初始化
来源：http://hz.shuidangran.top/gttasmvmxs.html


<!-- 参考信息 -->