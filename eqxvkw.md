代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhoulong.xyz/gtqxrnqarp.html

[Q54] 清空表
来源：http://hz.tanke756.top/gtlkwebdal.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtfzupggna.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtoyauiaku.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cashguo.top/gtnfznonft.html

[Q56] 密集排名（并列不占位）
来源：http://hz.mhx1999.top/gtoyiwoqjp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hammf.cn/gtegbcpqkk.html

[Q57] 行号
来源：http://hz.hnxiangtu.top/gteupribaf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtgaqjuaoj.html

[Q58] 累计求和
来源：http://hz.nanxinkj.top/gtljxgzipa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydjk.org.cn/gtaxmrrfza.html

[Q59] 分组内累计
来源：http://hz.chenlongwang.top/gtddaxmxwr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shzxlz.cn/gtuicakrpe.html

[Q60] 取上一行 / 下一行
来源：http://hz.sweek.top/gtbtyezgiy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtwrqwenof.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shuidangran.top/gtthgrqwla.html

[Q61] 移动平均
来源：http://hz.hnqzz.top/gtwnutfawn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtxkbjctsu.html

[Q62] 分组占比
来源：http://hz.guowangkeji.top/gtjrxfytda.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gtxffrsiyx.html

[Q63] 开启事务
来源：http://hz.smart0.xyz/gtrpxvjwoy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dashuyun.cn/gtbflsubub.html

[Q64] 提交事务
来源：http://hz.ppjwa.cn/gthyarrdgq.html

COMMIT;
来源：http://hz.c1oappe.top/gtrvzqterw.html

[Q65] 回滚事务
来源：http://hz.52xcode.cn/gtlwdssohe.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtulzvisgx.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtodmdksnu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangshuangyany.cn/gtuysenjja.html

[Q67] 设置隔离级别
来源：http://hz.ywan-chungtsiang.top/gtrozrucxj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gtziwcycch.html

[Q68] 保存点
来源：http://hz.gzhubu.top/gtkvzaxkcq.html

SAVEPOINT sp1;
来源：http://hz.cashguo.top/gtksvzwdaa.html

ROLLBACK TO sp1;
来源：http://hz.sweek.top/gtntwldcgc.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtrcttjlvm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yongpay.top/gtdkoctybc.html

[Q70] 更新统计信息
来源：http://hz.andypj.xyz/gtkqwvzmpc.html

ANALYZE TABLE users;
来源：http://hz.tianlin.xyz/gtdwyrxbug.html

[Q71] 查看建表语句
来源：http://hz.cqqwz.cn/gtyhyahsdy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cashguo.top/gtclzramua.html

[Q72] 查看索引
来源：http://hz.nanxuanxn.top/gttfmctawa.html

SHOW INDEX FROM users;
来源：http://hz.wangdashe.top/gtllsswlgy.html

[Q73] 查看表状态
来源：http://hz.ywan-chungtsiang.top/gtzfkprqgn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtdlcjjdmc.html

[Q74] 强制使用索引
来源：http://hz.yanxiufei.cn/gtplqgqult.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.haohaochexian.top/gtdgjpaxix.html

[Q75] 日期格式化
来源：http://hz.cheryme.top/gttocdtzre.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yonumen.top/gtzakwfxag.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.kuanghao11.cn/gtwovrongv.html

[Q76] 按天统计
来源：http://hz.chenzaomai.com/gtyhypsmii.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtqshviavn.html

[Q77] 时间加减
来源：http://hz.xinyue.icu/gtobebzesf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydzc1.top/gtpljfwuot.html

[Q78] 当前时间
来源：http://hz.xylfe.cn/gttwqrdbpp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gthipwyxnt.html

[Q79] 字符串拼接
来源：http://hz.yuanzhike.top/gtnoeqiltu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gtgemalskl.html

[Q80] 字符串截取
来源：http://hz.jinyuanbaomall.cn/gtyocemmnd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zdqjudy.top/gtmpxambna.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangtech.top/gtiwbkeacj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ppjwa.cn/gtsiscauum.html

[Q82] 字符长度与字节长度
来源：http://hz.daria6918.cn/gtqbfqntid.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtavqljdii.html

[Q83] 大小写转换
来源：http://hz.kuanghao11.cn/gtnrqmuyki.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jiagoushi.top/gtyndyqzgm.html

[Q84] 去除首尾空格
来源：http://hz.gogol.net.cn/gtjjkdohdn.html

SELECT TRIM(name) FROM users;
来源：http://hz.meibo888.top/gtiqjqxyti.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtdgfquors.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtwjuuamxx.html

[Q86] 读取 JSON 字段
来源：http://hz.fengsongda.top/gtfymzpwke.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.bjfxy.top/gtizmbmvjk.html

[Q87] JSON 字段做条件
来源：http://hz.hysaishi.cn/gtvkotmbku.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jqgfzy.top/gtlokwdabn.html

[Q88] 行转列（条件聚合）
来源：http://hz.jyoumei.cn/gtrlyedfgy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jyoumei.cn/gtwoyqsfcx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinghuilouyu.cn/gtdwxnferi.html

[Q89] 判断表是否存在
来源：http://hz.chenlongwang.top/gtvjwfbnva.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shzxlz.cn/gtgzynnhfq.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gthgduwvgi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aibaodan.cn/gtcgzfqsck.html

================================================================================
来源：http://hz.yongpay.top/gtsdedknke.html

R. Bash 专题
来源：http://hz.gogol.net.cn/gtgzxsqygt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtjmvikthh.html

[R01] shebang 与严格模式
来源：http://hz.haohaochexian.top/gtqvzgeqor.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gtlazixweu.html

set -euo pipefail
来源：http://hz.316326.xyz/gtbvhmvhzx.html

[R02] 变量赋值与使用
来源：http://hz.guowangkeji.top/gtsozzmmrb.html

name="Tom"; echo "$name"
来源：http://hz.svipenyu.cn/gtxnqsgdtf.html

[R03] 只读变量
来源：http://hz.redwolf501.top/gthowobtlv.html

readonly PI=3.14
来源：http://hz.zhongyouzk.top/gtzxngnidf.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtrobuhsiz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnqzz.top/gtvlftfgwb.html

[R05] 参数默认值
来源：http://hz.cucudq.cn/gtvhvppctw.html

name="${1:-default}"
来源：http://hz.aibaodan.cn/gtaxgdkkvt.html

[R06] 判断命令是否存在
来源：http://hz.yj20258888.top/gtxfnjyzce.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sweek.top/gtwpnraiiv.html

[R07] if 判断文件
来源：http://hz.yj202588.top/gtyjqbmrpq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yuxming.cn/gtbukpjmxt.html

[R08] 数值比较
来源：http://hz.cqqwz.cn/gtxsdhshme.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.snrcjt.cn/gtwgjpyqhp.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtfrxgpbnh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tanke756.top/gtpywujuiy.html

[R10] 正则匹配
来源：http://hz.pengpengdd.cyou/gtxxdcuphp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cdnleiting.top/gtcrrwnqce.html

[R11] case 多分支
来源：http://hz.gaohongyu789.top/gtbhalrwsn.html

case "$1" in
来源：http://hz.hfpthk.cn/gtxtshksnr.html

start) echo "启动" ;;
来源：http://hz.chenzaomai.com/gtpvvrujsi.html

stop)  echo "停止" ;;
来源：http://hz.ehwqpu.com/gtkgmycdza.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gthsunokdj.html

esac
来源：http://hz.gogol.net.cn/gtujmyfwir.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtpkenawun.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shanyushiyangtech.top/gtwqfdheig.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtqxctkstr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinghuilouyu.cn/gtrzwuoids.html

[R14] C 风格 for
来源：http://hz.yuanzhike.top/gtrzwxtgje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gtpeiijbil.html

[R15] while 逐行读文件
来源：http://hz.tanke756.top/gthofhbyxu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtzrpjzpde.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtvxgbghpd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.havefunace.top/gtwuhfvcnp.html

[R17] 数组定义与取值
来源：http://hz.andypj.xyz/gtdcuuwnxy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.52xcode.cn/gtokmkavgb.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtyhvwyude.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.snrcjt.cn/gtcskismxn.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtiqqaxfsq.html

echo "${#arr[@]}"
来源：http://hz.tianlin.xyz/gteautpmzy.html

[R20] 关联数组（字典）
来源：http://hz.yj202588.top/gtldhzdoyi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sysykeji.top/gttjsqjzhe.html

[R21] 字符串长度
来源：http://hz.jinyuanbaomall.cn/gtvgwzhuxt.html

echo "${#s}"
来源：http://hz.sysykeji.top/gtqxlkhqxg.html

[R22] 截取子串
来源：http://hz.yonumen.top/gtcoihrqnx.html

echo "${s:0:5}"
来源：http://hz.jinqigfzy.top/gtmkpqrdpa.html

[R23] 字符串替换
来源：http://hz.hywenlv.cn/gtosomtlcc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sweek.top/gthgvxvaxm.html

[R24] 大小写转换
来源：http://hz.nwbrower.top/gteoimqsab.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.snrcjt.cn/gthvumnluo.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtlcnrrnxd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinyuanbaomall.cn/gtcefzonao.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtuhxuttbj.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258.top/gtcqnflckq.html

[R27] 算术展开
来源：http://hz.daxiang520.top/gtmclgtyqi.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258888.top/gtztobdwoh.html

[R28] 浮点运算
来源：http://hz.zhixingplan.top/gtvgfylmol.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj202588.top/gtcjvjdqmx.html

[R29] 定义函数
来源：http://hz.svipenyu.cn/gtyuweepiw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuanzx.com/gtipfzttoq.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtzsuqcesy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.andypj.xyz/gtksevbwsj.html

[R31] 局部变量
来源：http://hz.quarkkingdee.top/gtvaryjcxg.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtqpikuckp.html

[R32] 参数个数校验
来源：http://hz.yuanzhike.top/gtqcfkxkop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gzhubu.top/gtsvcjkpjh.html

[R33] 捕获错误并提示行号
来源：http://hz.shzxlz.cn/gtahhwzepl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.andypj.xyz/gtqzkzyuns.html

[R34] 退出时清理
来源：http://hz.ppjwa.cn/gtiaeqmlvv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtcqcxfhap.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gtitcunxiv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtholicpul.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtfdwjqfia.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtfrwbmcqc.html

[R37] 把输出赋给变量
来源：http://hz.sxryk.cn/gtysleqasb.html

files=$(ls -1)
来源：http://hz.yuxming.cn/gtkmdypbld.html

[R38] 管道串联
来源：http://hz.aizwys.cn/gtvvjatwpr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pycfn.com/gtxlmcdmie.html

[R39] 重定向标准输出与错误
来源：http://hz.hongshengwenyu.top/gttxvamime.html

cmd > out.log 2>&1
来源：http://hz.aizwys.cn/gtoncmtfpd.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtkovqpctr.html

echo "log" >> out.log
来源：http://hz.xuanzx.com/gtuoyxjfvc.html

[R41] 丢弃输出
来源：http://hz.yuxming.cn/gtxybvheio.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtrjqoitpm.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtjdtnrepb.html

wc -l < a.txt
来源：http://hz.xuanzx.com/gtxrdcecku.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtwrhakytf.html

find . -name "*.log" -type f
来源：http://hz.yonumen.top/gtxixocosd.html

[R44] 按修改时间查找
来源：http://hz.cdnleiting.top/gtufrypxjw.html

find . -mtime -7 -type f
来源：http://hz.cqqwz.cn/gthnpszqcq.html

[R45] 批量删除
来源：http://hz.ehwqpu.com/gtbpbfncav.html

find . -name "*.tmp" -delete
来源：http://hz.meibo888.top/gtvjmanfku.html

[R46] 递归替换文件内容
来源：http://hz.gzhubu.top/gtkjxaefta.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aizwys.cn/gtzyqujncz.html

[R47] sed 单行替换
来源：http://hz.xziqi.cn/gtltdliqra.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cashguo.top/gtqajjfxid.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gtfplimklx.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gttdywqicf.html

[R49] awk 带条件
来源：http://hz.xuetiantiany.cn/gtfwrkrzxh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aizwys.cn/gtrkgbeoxf.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtumvbmdbr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.haohaochexian.top/gtxaoxopwi.html

[R51] 排序去重取前几
来源：http://hz.guannengcc.top/gtmfvbzhve.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.havefunace.top/gtoutrybdp.html

[R52] 统计行数
来源：http://hz.svipenyu.cn/gtiezgefnb.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtvcrsvaqz.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtabzbvyao.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtjivlaccf.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gtuqkjzbat.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gtqwztzcgv.html

[R55] 压缩与解压
来源：http://hz.guannengcc.top/gtwuqcxuiq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenjidiqi.icu/gtckclvlrl.html

[R56] 远程拷贝
来源：http://hz.hnqzz.top/gtkmkpnsne.html

scp file user@host:/path/
来源：http://hz.quarkkingdee.top/gtpmcmwhkp.html

[R57] 远程执行命令
来源：http://hz.zycfv.cn/gtjxmaheze.html

ssh user@host 'uptime'
来源：http://hz.yongpay.top/gttvlypmej.html

[R58] 下载文件
来源：http://hz.haohaochexian.top/gtksxgjhoo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtjjbycfph.html

[R59] 发 POST JSON
来源：http://hz.redwolf501.top/gthipkrtro.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pycfn.com/gtwucfokax.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydzc1.top/gtkkalafwa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tanke756.top/gtwswxpbgk.html

[R61] 磁盘占用
来源：http://hz.zhoulong.xyz/gtusyqmbdf.html

df -h;  du -sh *
来源：http://hz.wangshuangyany.cn/gtzxichzmn.html

[R62] 找最占空间的文件
来源：http://hz.yuxming.cn/gtgspllsbg.html

du -ah . | sort -rh | head -10
来源：http://hz.9152youxi.cn/gtregvunqo.html

[R63] 内存与进程
来源：http://hz.guowangkeji.top/gtpwfposhx.html

free -h;  ps aux | grep nginx
来源：http://hz.jlsjyb.cn/gtugpvdksj.html

[R64] 结束进程
来源：http://hz.yuanzhike.top/gtbxbjoqea.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cheryme.top/gtawuaxkjy.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtstbznxna.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangkeji.top/gtrtycualn.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtsnchjarl.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangtech.top/gthpxuagla.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gtqqlazfqy.html

openssl rand -hex 16
来源：http://hz.ydzc1.top/gtiznccepo.html

[R68] 计算文件校验值
来源：http://hz.hywenlv.cn/gtwaseegdm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gttjlezcvs.html

[R69] 生成随机密码
来源：http://hz.xziqi.cn/gtfyoetkfv.html

head -c 16 /dev/urandom | base64
来源：http://hz.fengsongda.top/gteekhclru.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtbtvaryfo.html

date +%s;  date -d @1700000000
来源：http://hz.nwbrower.top/gtjjjoymjo.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gtmbgyopdi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.birdmap.top/gtdfvleskx.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gtyvxcoaqu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shanyushiyangtech.top/gtnqrtmhjh.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtoqsojpwb.html

split -l 1000 big.log part_
来源：http://hz.shzxlz.cn/gtmrbdwcyv.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtluqyrwib.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yuxming.cn/gtlbkhdswl.html

[R75] 导出环境变量
来源：http://hz.jqgufenzy.top/gtcyamrutg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gthucqyvqm.html

[R76] 使用临时文件
来源：http://hz.nanxuanxn.top/gtsiqbftvs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jyoumei.cn/gtozbkubgh.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gtbywampnw.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtrrdjhwbc.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtqpuzodoy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtpcmgghjh.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtyixjmyxg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hysaishi.cn/gtdlvxrujy.html

[R80] 查看脚本执行耗时
来源：http://hz.shzxlz.cn/gthwdqiuri.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtwthbwcrn.html

================================================================================
来源：http://hz.xylfe.cn/gtjpzeigya.html

S. C / C++ 专题
来源：http://hz.xuanzx.com/gtnenfuayc.html

================================================================================
来源：http://hz.bjfxy.top/gtuosqtplr.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtccyjxrpl.html

#include <stdio.h>
来源：http://hz.haohaochexian.top/gtvpkfpnxt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinghuilouyu.cn/gtsrmxolql.html

[S02] C：变量与格式化输出
来源：http://hz.andypj.xyz/gtjxlzgcmx.html

int a = 10; printf("%d\n", a);
来源：http://hz.xingfuxueyuan.xyz/gtralrktmk.html

[S03] C：读入整数
来源：http://hz.jinqigfzy.top/gttuffmqmv.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gtyammzeet.html

[S04] C：字符串复制
来源：http://hz.sxryk.cn/gtrlzbvbne.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ywan-chungtsiang.top/gteljifadg.html

[S05] C：字符串长度
来源：http://hz.daria6918.cn/gttsbviobe.html

strlen(s)
来源：http://hz.ydjk.org.cn/gtvntyndcx.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gtubahcibz.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gtuyoiuabr.html

[S07] C：数组遍历求和
来源：http://hz.nwbrower.top/gtwfyrzgbn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fengsongda.top/gtzmutlnin.html

[S08] C：动态内存分配与释放
来源：http://hz.shangyingyoupin.top/gtaqdkwcjc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tianlin.xyz/gtjpxfwtmd.html

[S09] C：结构体定义与初始化
来源：http://hz.zycfv.cn/gtcggtulyb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtobsjnykx.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtdzjmnpus.html

int *p = &a;  *p = 5;
来源：http://hz.chenlongwang.top/gtabyyfbls.html

[S11] C：逐行读文件
来源：http://hz.fengsongda.top/gtnmckmngu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yuanzhike.top/gthpzkopwm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jianghu66.top/gtwmfasins.html

fclose(f);
来源：http://hz.gzhubu.top/gtbxcfyhyg.html

[S12] C：写文件
来源：http://hz.fzhhl.top/gtgliivubu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.svipenyu.cn/gtpcbxmjfw.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtnxpfkcua.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gtdpupgckd.html

[S14] C：枚举
来源：http://hz.jqgufenzy.top/gtqdsfgcza.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yangfankeji.com/gtzvvyevcv.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gtdxkpqyzk.html

(double) a / b
来源：http://hz.pengpengdd.cyou/gtjtdoopsz.html

[S16] C：位操作置位
来源：http://hz.gogol.net.cn/gtvsckqugp.html

x |= (1 << 3);
来源：http://hz.hongshengwenyu.top/gtxbmdulzf.html

[S17] C：安全拼接字符串
来源：http://hz.c1oappe.top/gtpbizohyt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgufenzy.top/gtknicrehb.html

[S18] C：命令行参数
来源：http://hz.nwbrower.top/gtbznndzji.html

int main(int argc, char **argv)
来源：http://hz.jinqigfzy.top/gtblzxnwqw.html

[S19] C：快速排序
来源：http://hz.nwbrower.top/gtkgxymbdv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtyzqfdclr.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtkhtpmatv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtivnrfaxn.html

[S21] C：字符类别判断
来源：http://hz.shuidangran.top/gtlweugfgx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.vqdsnc.cn/gtyeqrptmt.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtxdctoaid.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hysaishi.cn/gtmwcfzyjr.html

[S23] C：随机数
来源：http://hz.chenlongwang.top/gtxdldkwks.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtfqytcgjr.html

[S24] C：获取本地时间
来源：http://hz.mhx1999.top/gtpoqeenhh.html


<!-- 参考信息 -->