代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydzc1.top/gtowxudekv.html

[Q52] 删除指定行
来源：http://hz.wangshuangyany.cn/gttqslalbb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenzaomai.com/gtyozbnjkq.html

[Q53] 按条件删除
来源：http://hz.zdqjudy.top/gtvyojchyb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ywan-chungtsiang.top/gtrtwhksuf.html

[Q54] 清空表
来源：http://hz.wangshuangyany.cn/gtlgewnxto.html

TRUNCATE TABLE logs;
来源：http://hz.feifeiyinyue.top/gtimpjvneu.html

[Q55] 排名（并列占位）
来源：http://hz.hammf.cn/gtsbzdemni.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.meibo888.top/gtsboappwl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.0kj1m.cn/gtgumsfapm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuanzhike.top/gtxkwxjope.html

[Q57] 行号
来源：http://hz.meibo888.top/gtswydhpbe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ehwqpu.com/gteyctfiox.html

[Q58] 累计求和
来源：http://hz.yueranfly.top/gtkityihig.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pengpengdd.cyou/gtzvomador.html

[Q59] 分组内累计
来源：http://hz.snrcjt.cn/gtdscjifss.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangshuangyany.cn/gtuthromih.html

[Q60] 取上一行 / 下一行
来源：http://hz.sufxvd.cn/gtvrjrsgxq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gterwzxvzy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtkgekkjke.html

[Q61] 移动平均
来源：http://hz.xingfuxueyuan.xyz/gtwpwnited.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gtznugfaxw.html

[Q62] 分组占比
来源：http://hz.fengsongda.top/gtwslkqdgz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtgcpsabdy.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gthpmblzsn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangkeji.top/gtbnqxmnmw.html

[Q64] 提交事务
来源：http://hz.hnqzz.top/gtqkltjieg.html

COMMIT;
来源：http://hz.yuanzhike.top/gtqnkxnrpk.html

[Q65] 回滚事务
来源：http://hz.hongshengwenyu.top/gtilgzocny.html

ROLLBACK;
来源：http://hz.daria6918.cn/gtafngcfzj.html

[Q66] 行锁查询
来源：http://hz.xingfuxueyuan.xyz/gtuvntqdcu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cashguo.top/gtptwrrsit.html

[Q67] 设置隔离级别
来源：http://hz.chenzaomai.com/gtihyvoefj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.birdmap.top/gtdmgilylp.html

[Q68] 保存点
来源：http://hz.cqqwz.cn/gtdmaigoma.html

SAVEPOINT sp1;
来源：http://hz.yonumen.top/gtyebcsgto.html

ROLLBACK TO sp1;
来源：http://hz.cqqwz.cn/gtsrcrgnum.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtpwajygta.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhoulong.xyz/gttuoxozyl.html

[Q70] 更新统计信息
来源：http://hz.yuxming.cn/gtegyqkapx.html

ANALYZE TABLE users;
来源：http://hz.gaohongyu789.top/gtzpujjnir.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtjwbkuihp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtjpiqxlzq.html

[Q72] 查看索引
来源：http://hz.nanxuanxn.top/gtmcavmmah.html

SHOW INDEX FROM users;
来源：http://hz.yuxming.cn/gtafxwlmgk.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gthnlxykhq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pycfn.com/gtmfoczjxx.html

[Q74] 强制使用索引
来源：http://hz.shuidangran.top/gtgmxtedvk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhoulong.xyz/gtiiexfkrx.html

[Q75] 日期格式化
来源：http://hz.vqdsnc.cn/gtmhuurlqq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.svipenyu.cn/gtznrphodf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gaohongyu789.top/gtfctyhqpl.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtmevgfuqm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gtgxgymxtq.html

[Q77] 时间加减
来源：http://hz.sxryk.cn/gtxfalnzou.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtmljzpahj.html

[Q78] 当前时间
来源：http://hz.hywenlv.cn/gthdiibebz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinyuanbaomall.cn/gtipnwtkgp.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtihxcnkuz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.svipenyu.cn/gtmgqmbaxy.html

[Q80] 字符串截取
来源：http://hz.cashguo.top/gtqqhpazpl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.snrcjt.cn/gtzfcdejge.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtsmadlswe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daria6918.cn/gtlyyrrskk.html

[Q82] 字符长度与字节长度
来源：http://hz.ppjwa.cn/gtaoulpbrh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cqqwz.cn/gttvxjxonf.html

[Q83] 大小写转换
来源：http://hz.hnxiangtu.top/gtbjatwepe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.redwolf501.top/gtsfgajwta.html

[Q84] 去除首尾空格
来源：http://hz.hnxiangtu.top/gtopcqcyzu.html

SELECT TRIM(name) FROM users;
来源：http://hz.yongpay.top/gtjxnefomt.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtsgsvmmwk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.snrcjt.cn/gtqvfgfjlo.html

[Q86] 读取 JSON 字段
来源：http://hz.guannengcc.top/gtxkdkkaau.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.pengpengdd.cyou/gttoimhjhd.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtkgigpzai.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.andypj.xyz/gttlnzpznq.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenjidiqi.icu/gtmyqofjsz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nwbrower.top/gtnxvxregf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtobwuwbgr.html

[Q89] 判断表是否存在
来源：http://hz.nanxuanxn.top/gtyypamtuw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtlmkmtxus.html

[Q90] 生成序号列
来源：http://hz.sweek.top/gtzbymdfuk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenlongwang.top/gtncdbkdhx.html

================================================================================
来源：http://hz.dianchejie.cn/gtlfilytsu.html

R. Bash 专题
来源：http://hz.andypj.xyz/gtfgbcimlt.html

================================================================================
来源：http://hz.hammf.cn/gtxsznlwcu.html

[R01] shebang 与严格模式
来源：http://hz.0kj1m.cn/gttczzgycl.html

#!/usr/bin/env bash
来源：http://hz.jinghuilouyu.cn/gtnehbmqyg.html

set -euo pipefail
来源：http://hz.jlsjyb.cn/gtotimloqk.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gthtvvmsvu.html

name="Tom"; echo "$name"
来源：http://hz.cucudq.cn/gtoctljtft.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gtroqxiewx.html

readonly PI=3.14
来源：http://hz.cqqwz.cn/gtfzepdveh.html

[R04] 位置参数
来源：http://hz.chenjidiqi.icu/gttritrjgg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guowangkeji.top/gtzuxjvpto.html

[R05] 参数默认值
来源：http://hz.nanxinkj.top/gtzchxpiwc.html

name="${1:-default}"
来源：http://hz.zhijiandao.cn/gtybskblsr.html

[R06] 判断命令是否存在
来源：http://hz.yvedp.cn/gtjyujuzpv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenlongwang.top/gtvqjjjchd.html

[R07] if 判断文件
来源：http://hz.sufxvd.cn/gtnwfujvvv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shzxlz.cn/gteaiyxarq.html

[R08] 数值比较
来源：http://hz.chenjidiqi.icu/gtnvtncxbc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gtpsnqskqd.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtmgekvcut.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuanzx.com/gtbuzzuywq.html

[R10] 正则匹配
来源：http://hz.ydjk.org.cn/gtlbrtjblk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtdffxebyq.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtkmdhbsuk.html

case "$1" in
来源：http://hz.zdqjudy.top/gtzexbtaqr.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gtxvjxerby.html

stop)  echo "停止" ;;
来源：http://hz.aibaodan.cn/gtbeamjngx.html

*)     echo "未知命令" ;;
来源：http://hz.xylfe.cn/gtizdkdrfv.html

esac
来源：http://hz.guowangkeji.top/gtrqgocuvo.html

[R12] for 遍历文件
来源：http://hz.daxiang520.top/gtsmuxotmb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigufen.top/gtfxwnvlch.html

[R13] for 计数循环
来源：http://hz.xylfe.cn/gtiphpelhf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.chenzaomai.com/gtgavauhvz.html

[R14] C 风格 for
来源：http://hz.ybcxt.top/gtkdwjkerv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhixingplan.top/gtgazmgnzk.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtrfjaicfd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dianchejie.cn/gtobeviboe.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtuysfaaqr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtkxjxoief.html

[R17] 数组定义与取值
来源：http://hz.wangshuangyany.cn/gtdypavnxo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pengpengdd.cyou/gtvbvvpjrf.html

[R18] 遍历数组
来源：http://hz.9152youxi.cn/gtwlmzzfbq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtrdljozsk.html

[R19] 数组长度
来源：http://hz.jinqigfzy.top/gtajnfesqk.html

echo "${#arr[@]}"
来源：http://hz.hywenlv.cn/gtpajuosnu.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtszozkwqj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daxiang520.top/gtvhemdfmf.html

[R21] 字符串长度
来源：http://hz.mhx1999.top/gtcirdwdzw.html

echo "${#s}"
来源：http://hz.vqdsnc.cn/gtamlssest.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtzdlmgwwx.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtxknxhfbl.html

[R23] 字符串替换
来源：http://hz.wangdashe.top/gtgdbzpwmp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cqqwz.cn/gtlthqrnou.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtvzxwflqg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gogol.net.cn/gtutrebooy.html

[R25] 去后缀 / 去前缀
来源：http://hz.yvedp.cn/gtkpxwaxwu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cashguo.top/gtjdpdssfc.html

[R26] 命令替换
来源：http://hz.zhengqikj.top/gtzrehmobe.html

now=$(date +%F); echo "$now"
来源：http://hz.ywan-chungtsiang.top/gtkuclfxvt.html

[R27] 算术展开
来源：http://hz.shanyushiyangkeji.top/gtlzcxnocr.html

echo $((1 + 2 * 3))
来源：http://hz.kuanghao11.cn/gtdirlpqsm.html

[R28] 浮点运算
来源：http://hz.aibaodan.cn/gtkjfraruo.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangkeji.top/gtgjfeucdw.html

[R29] 定义函数
来源：http://hz.pycfn.com/gtsetvxice.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtiibbixrz.html

[R30] 函数返回状态码
来源：http://hz.yuanzhike.top/gtzsxrcpgl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xinyue.icu/gtrkpxufxx.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gtzayyniqw.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtybetwcos.html

[R32] 参数个数校验
来源：http://hz.mhx1999.top/gtlfzyfhiw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtvxzszxuq.html

[R33] 捕获错误并提示行号
来源：http://hz.zhengqikj.top/gtzzbcvxgs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jyoumei.cn/gtkdttfvwk.html

[R34] 退出时清理
来源：http://hz.xylfe.cn/gtzeabukrl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtyjmwrwac.html

[R35] 后台执行并等待
来源：http://hz.svipenyu.cn/gthedjcsjy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shangyingyoupin.top/gtcdzebujj.html

[R36] 并发执行多个任务
来源：http://hz.tanke756.top/gtrvtcyorc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhengqikj.top/gtejdmqkpy.html

[R37] 把输出赋给变量
来源：http://hz.hammf.cn/gtazokcyfh.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtrljiadgx.html

[R38] 管道串联
来源：http://hz.havefunace.top/gtnqqyllbr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gotoacloud.top/gtdjlckvst.html

[R39] 重定向标准输出与错误
来源：http://hz.jiagoushi.top/gtbedlcvtv.html

cmd > out.log 2>&1
来源：http://hz.yvedp.cn/gtrkolbgiy.html

[R40] 追加写日志
来源：http://hz.daria6918.cn/gtggxjpjnq.html

echo "log" >> out.log
来源：http://hz.nanxuanxn.top/gtugtebswf.html

[R41] 丢弃输出
来源：http://hz.yuxming.cn/gtcgctumjg.html

cmd >/dev/null 2>&1
来源：http://hz.jyoumei.cn/gtuhhusjao.html

[R42] 输入重定向
来源：http://hz.shanyushiyangtech.top/gtogghqmvt.html

wc -l < a.txt
来源：http://hz.kuanghao11.cn/gtldfanzsg.html

[R43] 按名字查找文件
来源：http://hz.snrcjt.cn/gtbmjkwute.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gtfkwzdjxm.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtumfufdgn.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtnfgmmkgr.html

[R45] 批量删除
来源：http://hz.sxryk.cn/gtntkbcqhw.html

find . -name "*.tmp" -delete
来源：http://hz.cdnleiting.top/gttmecgbph.html

[R46] 递归替换文件内容
来源：http://hz.aibaodan.cn/gthrgaicfr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pengpengdd.cyou/gtqmjufigl.html

[R47] sed 单行替换
来源：http://hz.yuxming.cn/gtvhcvottn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sufxvd.cn/gtrnhbctsp.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtjqtnsylk.html

awk '{print $1, $3}' a.txt
来源：http://hz.0kj1m.cn/gtsthvsbcx.html

[R49] awk 带条件
来源：http://hz.yangfankeji.com/gthnadluyy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sufxvd.cn/gtjnufzdfh.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtqjupokqy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtufoecbwq.html

[R51] 排序去重取前几
来源：http://hz.316326.xyz/gtqzsrqtik.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zdqjudy.top/gtvlgmtpcy.html

[R52] 统计行数
来源：http://hz.nwbrower.top/gtiapuymjr.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gttdjofaok.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtolbyjgfh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhixingplan.top/gtacrlzkxf.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtqfipjoru.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gtiffjfqiw.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtqzertcch.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shuidangran.top/gtxrtqiruz.html

[R56] 远程拷贝
来源：http://hz.zdqjudy.top/gtthztpzwl.html

scp file user@host:/path/
来源：http://hz.hysaishi.cn/gtzjfvjyvk.html

[R57] 远程执行命令
来源：http://hz.xuetiantiany.cn/gtkepqgijj.html

ssh user@host 'uptime'
来源：http://hz.ydjk.org.cn/gtryepehan.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtkfnrdcxt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtkfcflcyh.html

[R59] 发 POST JSON
来源：http://hz.daria6918.cn/gtoptlikwh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ivvv.top/gtxozuamhv.html

[R60] 只看 HTTP 状态码
来源：http://hz.smart0.xyz/gtinxcbhvu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhiwuduotai.top/gtbylmthmw.html

[R61] 磁盘占用
来源：http://hz.yangfankeji.com/gtddneuaos.html

df -h;  du -sh *
来源：http://hz.zhongyouzk.top/gtfccxygjp.html

[R62] 找最占空间的文件
来源：http://hz.jiagoushi.top/gtxmnumxwj.html

du -ah . | sort -rh | head -10
来源：http://hz.jianghu66.top/gtsogqzieo.html

[R63] 内存与进程
来源：http://hz.shangyingyoupin.top/gtpwsnabjd.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxuanxn.top/gtomsjjybu.html

[R64] 结束进程
来源：http://hz.sweek.top/gtixrryqux.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtjlexyywg.html

[R65] 查看端口占用
来源：http://hz.yuanzhike.top/gthabikgqe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtiomtxrkc.html

[R66] 定时任务
来源：http://hz.fzhhl.top/gtwclkyjuy.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtwjdavpro.html

[R67] 生成随机十六进制串
来源：http://hz.hnqzz.top/gtdmzyravx.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtbmkwogim.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtsdnddidq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtctyjiotz.html

[R69] 生成随机密码
来源：http://hz.sufxvd.cn/gtxnukzpum.html

head -c 16 /dev/urandom | base64
来源：http://hz.aibaodan.cn/gtpzgiazwl.html

[R70] 时间戳与互转
来源：http://hz.9152youxi.cn/gtmevjbmoj.html

date +%s;  date -d @1700000000
来源：http://hz.cucudq.cn/gtgznhnbno.html

[R71] 日期格式化
来源：http://hz.fengsongda.top/gtyitfwjli.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cqqwz.cn/gtcwaszgtv.html

[R72] 等待端口就绪
来源：http://hz.jinqigfzy.top/gtkrmzoxqj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.9152youxi.cn/gtywokdsgo.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtnxaxdyxt.html

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtojghqjvt.html

[R74] 批量重命名
来源：http://hz.hfpthk.cn/gtfjmvcjrz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigufen.top/gtiowlpabq.html

[R75] 导出环境变量
来源：http://hz.zhaomingkeji.xyz/gtizhtjvtl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gtcejpbgdm.html

[R76] 使用临时文件
来源：http://hz.316326.xyz/gtvwmdscbz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtecrcnljp.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gttqqmshpc.html

read -rp "请输入: " ans
来源：http://hz.smart0.xyz/gtpbbzmswm.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtdtqlpwqq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.quarkkingdee.top/gtrtgwyiwc.html

[R79] 解析命令行选项
来源：http://hz.nanxuanxn.top/gtloxdaaur.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jiagoushi.top/gtbwxnzypd.html

[R80] 查看脚本执行耗时
来源：http://hz.yvedp.cn/gtezphbeuc.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtnzovlgdz.html

================================================================================
来源：http://hz.guannengcc.top/gtmwscbhxy.html

S. C / C++ 专题
来源：http://hz.wangdashe.top/gtqvxohhkj.html

================================================================================
来源：http://hz.yueranfly.top/gtstvikvek.html

[S01] C：Hello World
来源：http://hz.yj20258.top/gtvkbrwpig.html

#include <stdio.h>
来源：http://hz.meibo888.top/gtxasaujll.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hongshengwenyu.top/gtpejhmtyv.html

[S02] C：变量与格式化输出
来源：http://hz.vqdsnc.cn/gtfvykfzki.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuetiantiany.cn/gteaehtkca.html

[S03] C：读入整数
来源：http://hz.aizwys.cn/gtciczzzfe.html

int x; scanf("%d", &x);
来源：http://hz.jyoumei.cn/gtruhsazhg.html

[S04] C：字符串复制
来源：http://hz.svipenyu.cn/gtzqxbbqox.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jlsjyb.cn/gtfcobibjy.html

[S05] C：字符串长度
来源：http://hz.316326.xyz/gtvicwluan.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtuxlydhbg.html

[S06] C：字符串比较
来源：http://hz.dianchejie.cn/gtewyosecy.html

strcmp(a, b) == 0
来源：http://hz.yueranfly.top/gthuwfhqlp.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gtjhjshbxu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnxiangtu.top/gtydliestq.html

[S08] C：动态内存分配与释放
来源：http://hz.sxryk.cn/gtibwoxxmq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtbaaunvkx.html

[S09] C：结构体定义与初始化
来源：http://hz.zhiwuduotai.top/gtkrykghtk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.havefunace.top/gttsdhjtpk.html

[S10] C：指针与解引用
来源：http://hz.meibo888.top/gtmnlnuxet.html

int *p = &a;  *p = 5;
来源：http://hz.bjfxy.top/gtzraoihfs.html

[S11] C：逐行读文件
来源：http://hz.meibo888.top/gtuyfioudn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daria6918.cn/gtsebigxab.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydjk.org.cn/gtzhlqenkz.html

fclose(f);
来源：http://hz.ybcxt.top/gtlykgpkta.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtvadmnifv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhiwuduotai.top/gtuosrbjvr.html

[S13] C：宏定义
来源：http://hz.0kj1m.cn/gtiojutmjz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtrqpjihvm.html

[S14] C：枚举
来源：http://hz.feifeiyinyue.top/gtjvenjbyx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jyoumei.cn/gtmfdixhfu.html

[S15] C：类型转换
来源：http://hz.cucudq.cn/gtvozcdbkw.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtfdnwquxx.html

[S16] C：位操作置位
来源：http://hz.cqqwz.cn/gthcpehbhp.html

x |= (1 << 3);
来源：http://hz.gotoacloud.top/gtkhxkrxui.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtixgckwow.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.c1oappe.top/gtraltfapc.html

[S18] C：命令行参数
来源：http://hz.jinqigufen.top/gtdvvvsbhw.html

int main(int argc, char **argv)
来源：http://hz.c1oappe.top/gtotjidlqv.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtrfgyiciu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtevtptevg.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtwnlcxlne.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gttwsnsywq.html

[S21] C：字符类别判断
来源：http://hz.andypj.xyz/gtwqxyssex.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258888.top/gtwtmogbjb.html

[S22] C：字符串转数字
来源：http://hz.ywan-chungtsiang.top/gtgohhtcbi.html


<!-- 参考信息 -->