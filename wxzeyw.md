代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gotoacloud.top/gthwljagke.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gtrcywiuov.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtsgtbclpk.html

[Q59] 分组内累计
来源：http://hz.xylfe.cn/gtvzyfwwst.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gthwcfwbbb.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtitomgrve.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shuidangran.top/gtnadgfzfp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gaohongyu789.top/gtvcupdqlm.html

[Q61] 移动平均
来源：http://hz.tianlin.xyz/gtmdnfwviq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shzxlz.cn/gtynduriyb.html

[Q62] 分组占比
来源：http://hz.zhongyouzk.top/gtxgfgbavx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtraqbyqqd.html

[Q63] 开启事务
来源：http://hz.ppjwa.cn/gtenkbgjry.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cucudq.cn/gtsmticsou.html

[Q64] 提交事务
来源：http://hz.birdmap.top/gtcrqpuhdm.html

COMMIT;
来源：http://hz.jyoumei.cn/gtcjpsvjuh.html

[Q65] 回滚事务
来源：http://hz.xylfe.cn/gtfonrnsjx.html

ROLLBACK;
来源：http://hz.redwolf501.top/gttiuursnu.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtkrpkzxzs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gtwgfbneum.html

[Q67] 设置隔离级别
来源：http://hz.zhongyouzk.top/gtogrxkuaa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gtxltrdlud.html

[Q68] 保存点
来源：http://hz.jyoumei.cn/gtdglnnzbx.html

SAVEPOINT sp1;
来源：http://hz.aizwys.cn/gtomvattyv.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gttkcwnzwq.html

[Q69] 查看执行计划
来源：http://hz.zhixingplan.top/gttlxyqfwo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.52xcode.cn/gtlohzfmiv.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gthbxhzpjd.html

ANALYZE TABLE users;
来源：http://hz.xylfe.cn/gttwvdjqrg.html

[Q71] 查看建表语句
来源：http://hz.hnxiangtu.top/gttmkdpkuj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tanke756.top/gtxtbvngyt.html

[Q72] 查看索引
来源：http://hz.ehwqpu.com/gtdvusqlzp.html

SHOW INDEX FROM users;
来源：http://hz.jinyuanbaomall.cn/gtuwxcuplp.html

[Q73] 查看表状态
来源：http://hz.jqgfzy.top/gtmhcdicua.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daria6918.cn/gttgoducfo.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtyayvzton.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hywenlv.cn/gtodiphspo.html

[Q75] 日期格式化
来源：http://hz.andypj.xyz/gthsbsnrjz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.haohaochexian.top/gthbwyguio.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ywan-chungtsiang.top/gtejvfgafq.html

[Q76] 按天统计
来源：http://hz.wangshuangyany.cn/gtfojyzhgy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.feifeiyinyue.top/gtccwshmgd.html

[Q77] 时间加减
来源：http://hz.yangfankeji.com/gtuswuwczm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenlongwang.top/gtwvwuagpj.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtacpiwncj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yangfankeji.com/gtjerwdlwp.html

[Q79] 字符串拼接
来源：http://hz.c1oappe.top/gtplsezeab.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangdashe.top/gtfmpqhbjg.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gtvhlszess.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.kuanghao11.cn/gtoofmwyrr.html

[Q81] 字符串替换
来源：http://hz.haohaochexian.top/gtxkvsnjru.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yonumen.top/gtokfnoyen.html

[Q82] 字符长度与字节长度
来源：http://hz.guowangkeji.top/gthmkfuade.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtfpecgrqi.html

[Q83] 大小写转换
来源：http://hz.zhaomingkeji.xyz/gtnkfwywxg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gtkbsjnuae.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtupjflojf.html

SELECT TRIM(name) FROM users;
来源：http://hz.tian-w.cn/gtqoakwisi.html

[Q85] 数值取整
来源：http://hz.aibaodan.cn/gtbqqsmxxp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guannengcc.top/gtvlkxueid.html

[Q86] 读取 JSON 字段
来源：http://hz.cdnleiting.top/gtytrncewq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinyuanbaomall.cn/gtbjgucquv.html

[Q87] JSON 字段做条件
来源：http://hz.jianghu66.top/gtrzhypwbq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tanke756.top/gtuvxmftqp.html

[Q88] 行转列（条件聚合）
来源：http://hz.sufxvd.cn/gtpokulmbk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtqykqmsfu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydjk.org.cn/gtyrvwxwoy.html

[Q89] 判断表是否存在
来源：http://hz.zhiwuduotai.top/gtenlwxnha.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.bjfxy.top/gtbwyxxstq.html

[Q90] 生成序号列
来源：http://hz.zhaomingkeji.xyz/gtbwgkrujx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.0kj1m.cn/gtltbgbrxx.html

================================================================================
来源：http://hz.xziqi.cn/gttuosqmry.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtsberrmbm.html

================================================================================
来源：http://hz.aibaodan.cn/gtsdyfdnjk.html

[R01] shebang 与严格模式
来源：http://hz.9152youxi.cn/gtqnsrcrit.html

#!/usr/bin/env bash
来源：http://hz.316326.xyz/gtiragjvdh.html

set -euo pipefail
来源：http://hz.tian-w.cn/gtkyogiutm.html

[R02] 变量赋值与使用
来源：http://hz.pengpengdd.cyou/gtefmnjsfz.html

name="Tom"; echo "$name"
来源：http://hz.birdmap.top/gtebhxihel.html

[R03] 只读变量
来源：http://hz.gzhubu.top/gtqdtpmkfv.html

readonly PI=3.14
来源：http://hz.xingfuxueyuan.xyz/gtdkfqkoqn.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtdbbeotyc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xylfe.cn/gtkdizlcbv.html

[R05] 参数默认值
来源：http://hz.c1oappe.top/gtwtglpbud.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtfnxkymrb.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtcknvrgsz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtlumwijfl.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gtvyacivzf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gogol.net.cn/gtgksaxeor.html

[R08] 数值比较
来源：http://hz.zhiwuduotai.top/gtfuhlcgio.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258888.top/gtoiojtwxx.html

[R09] 字符串比较
来源：http://hz.hammf.cn/gtwcclwsxd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtzwclholo.html

[R10] 正则匹配
来源：http://hz.dianchejie.cn/gtqmlkodit.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhoulong.xyz/gtyniykxdg.html

[R11] case 多分支
来源：http://hz.yj202588.top/gtzoiqvbjg.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gtwaxzfnry.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gtnmnsmmvv.html

stop)  echo "停止" ;;
来源：http://hz.tanke756.top/gtdzonqawh.html

*)     echo "未知命令" ;;
来源：http://hz.ywan-chungtsiang.top/gteqmwkeqc.html

esac
来源：http://hz.zhengqikj.top/gtldyzkmno.html

[R12] for 遍历文件
来源：http://hz.zhongyouzk.top/gtxfbaggon.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xingfuxueyuan.xyz/gtugxzbuhm.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtnydavyth.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtcgllcffc.html

[R14] C 风格 for
来源：http://hz.jinqigfzy.top/gtkucwlfdd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtccfipbxz.html

[R15] while 逐行读文件
来源：http://hz.xuetiantiany.cn/gtvroigupj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yueranfly.top/gtxasiojxs.html

[R16] until 等待条件
来源：http://hz.c1oappe.top/gtepvtdizb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gtfxmpcprw.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gtmeierxta.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.quarkkingdee.top/gtuflwxlxl.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtjymqvzpx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtzqlxbhgv.html

[R19] 数组长度
来源：http://hz.cucudq.cn/gtplxvlyvp.html

echo "${#arr[@]}"
来源：http://hz.wangshuangyany.cn/gtqtbwqrch.html

[R20] 关联数组（字典）
来源：http://hz.aizwys.cn/gthsanewwv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jianghu66.top/gtrfuycznv.html

[R21] 字符串长度
来源：http://hz.aizwys.cn/gtlvfuuhqd.html

echo "${#s}"
来源：http://hz.snrcjt.cn/gtiekmppmq.html

[R22] 截取子串
来源：http://hz.hnqzz.top/gtrmjudjzf.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtrpuvzgym.html

[R23] 字符串替换
来源：http://hz.shangyingyoupin.top/gtfzmmogco.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hywenlv.cn/gtetfbidvs.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtkhishxyn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gthhdrvudg.html

[R25] 去后缀 / 去前缀
来源：http://hz.ybcxt.top/gttvumjymj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhaomingkeji.xyz/gtnkokaiun.html

[R26] 命令替换
来源：http://hz.jinqigufen.top/gtgnxyevdo.html

now=$(date +%F); echo "$now"
来源：http://hz.havefunace.top/gtsjeeydkp.html

[R27] 算术展开
来源：http://hz.ywan-chungtsiang.top/gtinaaulmw.html

echo $((1 + 2 * 3))
来源：http://hz.nanxuanxn.top/gtcochuytv.html

[R28] 浮点运算
来源：http://hz.kuanghao11.cn/gtvcxainak.html

echo "scale=2; 10/3" | bc
来源：http://hz.gzhubu.top/gtzdmwtegi.html

[R29] 定义函数
来源：http://hz.yangfankeji.com/gtratdvhfs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.quarkkingdee.top/gtjxavqfqk.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gtrduxqupp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtpecigtvq.html

[R31] 局部变量
来源：http://hz.ppjwa.cn/gtudnjrjjr.html

f() { local x=1; echo "$x"; }
来源：http://hz.gzhubu.top/gtqqiwtpem.html

[R32] 参数个数校验
来源：http://hz.dianchejie.cn/gtcwctsuqo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtdanxnime.html

[R33] 捕获错误并提示行号
来源：http://hz.hongshengwenyu.top/gtmroaeadg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sufxvd.cn/gtjtgsuefv.html

[R34] 退出时清理
来源：http://hz.redwolf501.top/gttfcyehei.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgufenzy.top/gtcihzegup.html

[R35] 后台执行并等待
来源：http://hz.svipenyu.cn/gtdncsgmbc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pengpengdd.cyou/gtfbedfgbf.html

[R36] 并发执行多个任务
来源：http://hz.jinqigfzy.top/gtngaxmhlw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.feifeiyinyue.top/gtwghmxatm.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gtzbphyiah.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtueytkzsj.html

[R38] 管道串联
来源：http://hz.tianlin.xyz/gtqviberlj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtettdvjfp.html

[R39] 重定向标准输出与错误
来源：http://hz.dashuyun.cn/gtqwbhpckc.html

cmd > out.log 2>&1
来源：http://hz.zycfv.cn/gtayzwjeoy.html

[R40] 追加写日志
来源：http://hz.vqdsnc.cn/gtxrpvbbrk.html

echo "log" >> out.log
来源：http://hz.gogol.net.cn/gtfkpnoelz.html

[R41] 丢弃输出
来源：http://hz.guowangkeji.top/gtrakiuhol.html

cmd >/dev/null 2>&1
来源：http://hz.yvedp.cn/gtlzjpkrek.html

[R42] 输入重定向
来源：http://hz.ppjwa.cn/gthkmjahad.html

wc -l < a.txt
来源：http://hz.jinqigufen.top/gtvncbacqq.html

[R43] 按名字查找文件
来源：http://hz.zycfv.cn/gtyebwuvtm.html

find . -name "*.log" -type f
来源：http://hz.jinyuanbaomall.cn/gtcjezxgev.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gtnhnslvsg.html

find . -mtime -7 -type f
来源：http://hz.ppjwa.cn/gtddvpgwfo.html

[R45] 批量删除
来源：http://hz.sxryk.cn/gtbesbkdzj.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtfgapxyzw.html

[R46] 递归替换文件内容
来源：http://hz.tianlin.xyz/gtcxhzetei.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fengsongda.top/gteidiozyq.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtamvtcels.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gtdizdvaut.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtvgbbhwfw.html

awk '{print $1, $3}' a.txt
来源：http://hz.andypj.xyz/gtbpthkqbx.html

[R49] awk 带条件
来源：http://hz.cashguo.top/gtgscpsqve.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nwbrower.top/gtcknuoaan.html

[R50] awk 求和
来源：http://hz.ybcxt.top/gtdhzcuwet.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jlsjyb.cn/gtebklbsrt.html

[R51] 排序去重取前几
来源：http://hz.ydzc1.top/gtkpzxqfyz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtqgswswef.html

[R52] 统计行数
来源：http://hz.yj202588.top/gtsjzwqdgs.html

wc -l a.txt
来源：http://hz.jqgfzy.top/gtghlrfvjg.html

[R53] 查看文件头与实时尾
来源：http://hz.hysaishi.cn/gtwxufcqke.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.andypj.xyz/gtsnlqhfik.html

[R54] 比较两个文件
来源：http://hz.fzhhl.top/gtczbhcfjb.html

diff a.txt b.txt
来源：http://hz.zhiwuduotai.top/gtqjdavesr.html

[R55] 压缩与解压
来源：http://hz.cashguo.top/gtdwqytkkf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtpwzfgqhr.html

[R56] 远程拷贝
来源：http://hz.xingfuxueyuan.xyz/gtwagmsxuo.html

scp file user@host:/path/
来源：http://hz.jinqigfzy.top/gtwgfyoslx.html

[R57] 远程执行命令
来源：http://hz.cdnleiting.top/gtbexvimyt.html

ssh user@host 'uptime'
来源：http://hz.wangdashe.top/gtrldejiaa.html

[R58] 下载文件
来源：http://hz.c1oappe.top/gtwhytqtux.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.havefunace.top/gtqxvycpjt.html

[R59] 发 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtgrnynpdl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtlsbunvqt.html

[R60] 只看 HTTP 状态码
来源：http://hz.cheryme.top/gtxqhxzjbd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.c1oappe.top/gtbvwmydxq.html

[R61] 磁盘占用
来源：http://hz.andypj.xyz/gtwzpnjxfx.html

df -h;  du -sh *
来源：http://hz.havefunace.top/gtdkbhxfet.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtqmackiar.html

du -ah . | sort -rh | head -10
来源：http://hz.gaohongyu789.top/gtycvldxop.html

[R63] 内存与进程
来源：http://hz.zhaomingkeji.xyz/gtimeqgegz.html

free -h;  ps aux | grep nginx
来源：http://hz.fzhhl.top/gtnqmcrztz.html

[R64] 结束进程
来源：http://hz.chenzaomai.com/gttbsylglj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.snrcjt.cn/gtzggeojsj.html

[R65] 查看端口占用
来源：http://hz.ppjwa.cn/gtppskefbw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aizwys.cn/gtuecdmuwq.html

[R66] 定时任务
来源：http://hz.yanxiufei.cn/gttwozhwrf.html

crontab -e;  crontab -l
来源：http://hz.9152youxi.cn/gtpwfsprtn.html

[R67] 生成随机十六进制串
来源：http://hz.daria6918.cn/gtdurugdfk.html

openssl rand -hex 16
来源：http://hz.aibaodan.cn/gtecoihicm.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangtech.top/gtgifdytiw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.316326.xyz/gtpgpgapzl.html

[R69] 生成随机密码
来源：http://hz.fengsongda.top/gtqhxlyary.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhengqikj.top/gtrhvtxfsl.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtejffjchd.html

date +%s;  date -d @1700000000
来源：http://hz.yj202588.top/gtefitjbao.html

[R71] 日期格式化
来源：http://hz.birdmap.top/gtagmfjjov.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhiwuduotai.top/gtisfmqtaf.html

[R72] 等待端口就绪
来源：http://hz.nwbrower.top/gtzkykjjcw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtyapjbage.html

[R73] 分割大日志
来源：http://hz.jinqigufen.top/gtnovpnvgl.html

split -l 1000 big.log part_
来源：http://hz.zdqjudy.top/gtkwctwdny.html

[R74] 批量重命名
来源：http://hz.xinyue.icu/gtmwflasft.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ybcxt.top/gtyvxdlfnf.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gtfqwyvtix.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtrnqzfgqi.html

[R76] 使用临时文件
来源：http://hz.zhengqikj.top/gtbnadhfnv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtaehvurtj.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangkeji.top/gticpqrkwb.html

read -rp "请输入: " ans
来源：http://hz.jqgufenzy.top/gtwqwyfwmk.html

[R78] 交互式菜单
来源：http://hz.sxryk.cn/gtzvjaeqyj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtdozmgcpe.html

[R79] 解析命令行选项
来源：http://hz.hfpthk.cn/gtbzuppwhd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xziqi.cn/gtjgixngjr.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtcapwzrfr.html

time ./run.sh
来源：http://hz.ivvv.top/gtpcjbklmx.html

================================================================================
来源：http://hz.chenlongwang.top/gtzdzgxecd.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtpcvjhvru.html

================================================================================
来源：http://hz.cdnleiting.top/gtmpfvanoa.html

[S01] C：Hello World
来源：http://hz.ybcxt.top/gtaqxfgsjo.html

#include <stdio.h>
来源：http://hz.ywan-chungtsiang.top/gtryrbvylr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yonumen.top/gtiuykdwpy.html

[S02] C：变量与格式化输出
来源：http://hz.yonumen.top/gtgfvhejwr.html

int a = 10; printf("%d\n", a);
来源：http://hz.yonumen.top/gtxpzgpmpi.html

[S03] C：读入整数
来源：http://hz.yj20258.top/gtyncckunl.html

int x; scanf("%d", &x);
来源：http://hz.guowangkeji.top/gtopfbcrfa.html

[S04] C：字符串复制
来源：http://hz.yueranfly.top/gtkfsfmdyu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ivvv.top/gtjuexnekw.html

[S05] C：字符串长度
来源：http://hz.ywan-chungtsiang.top/gtacszmdpc.html

strlen(s)
来源：http://hz.shangyingyoupin.top/gtrdnaetxo.html

[S06] C：字符串比较
来源：http://hz.guannengcc.top/gtqhfagegm.html

strcmp(a, b) == 0
来源：http://hz.gaohongyu789.top/gtbzphzxjo.html

[S07] C：数组遍历求和
来源：http://hz.52xcode.cn/gtyqxghokw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangshuangyany.cn/gtcvmgcojr.html

[S08] C：动态内存分配与释放
来源：http://hz.ehwqpu.com/gtuynjxaow.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xingfuxueyuan.xyz/gtpocaotod.html

[S09] C：结构体定义与初始化
来源：http://hz.svipenyu.cn/gtqgcbhyls.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zdqjudy.top/gtezndhuas.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtjszomnkm.html

int *p = &a;  *p = 5;
来源：http://hz.jiagoushi.top/gtowsnsddp.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtlwducbjp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.svipenyu.cn/gtnqcngrow.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtuwstuswr.html

fclose(f);
来源：http://hz.jinghuilouyu.cn/gtputpwzpi.html

[S12] C：写文件
来源：http://hz.jyoumei.cn/gtjyaueurd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ivvv.top/gtztcepcht.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtrmazyenv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jlsjyb.cn/gtiihdgvhb.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gtbhjfktfi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nwbrower.top/gtnphnrqhe.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtzqtypepz.html

(double) a / b
来源：http://hz.pycfn.com/gtblgwthky.html

[S16] C：位操作置位
来源：http://hz.jinyuanbaomall.cn/gtxkjjvjqk.html

x |= (1 << 3);
来源：http://hz.zhengqikj.top/gtondfcgfy.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gteupzatbq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hnqzz.top/gtsujtoybn.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtxhioshlq.html

int main(int argc, char **argv)
来源：http://hz.0kj1m.cn/gtdzfjsoop.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtzmampxvx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtlhpvmgcd.html

[S20] C：二分查找
来源：http://hz.yj20258888.top/gtrurmteck.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtgxuiyudo.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtxefgdbjy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.fzhhl.top/gtdigjhyko.html

[S22] C：字符串转数字
来源：http://hz.xziqi.cn/gtauyfhlqp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cqqwz.cn/gtquvmfkpq.html

[S23] C：随机数
来源：http://hz.wangdashe.top/gtkxqlntso.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhaomingkeji.xyz/gtayqzkubh.html

[S24] C：获取本地时间
来源：http://hz.jinqigfzy.top/gtkmevlczq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydjk.org.cn/gtazdnqsjz.html

[S25] C：内存拷贝
来源：http://hz.xuetiantiany.cn/gtgamueruo.html

memcpy(dst, src, n);
来源：http://hz.vqdsnc.cn/gthvrgwhmg.html

[S26] C：内存清零
来源：http://hz.hnxiangtu.top/gtjnnxzfim.html

memset(a, 0, sizeof a);
来源：http://hz.hnxiangtu.top/gtojiezkzk.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gtinewelaq.html

const double PI = 3.14159;
来源：http://hz.tanke756.top/gtuutfkrak.html

[S28] C：静态变量
来源：http://hz.cashguo.top/gtylujixmu.html


<!-- 参考信息 -->