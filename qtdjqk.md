代发 wailian999

[Q63] 开启事务
来源：http://hz.hfpthk.cn/gtzkrrpmxf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhijiandao.cn/gttbzuhrlt.html

[Q64] 提交事务
来源：http://hz.zhaomingkeji.xyz/gtcrpaadlf.html

COMMIT;
来源：http://hz.sysykeji.top/gtdmqozgwt.html

[Q65] 回滚事务
来源：http://hz.cucudq.cn/gtkvjruips.html

ROLLBACK;
来源：http://hz.0kj1m.cn/gtqwdqcffp.html

[Q66] 行锁查询
来源：http://hz.meibo888.top/gtjltjybjd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yvedp.cn/gtjwofzcqx.html

[Q67] 设置隔离级别
来源：http://hz.ehwqpu.com/gtfpdfrxbz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhiwuduotai.top/gtrsdrbvnj.html

[Q68] 保存点
来源：http://hz.jinqigfzy.top/gtjplrpeym.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtdjxhurcy.html

ROLLBACK TO sp1;
来源：http://hz.shzxlz.cn/gtnfuclucd.html

[Q69] 查看执行计划
来源：http://hz.vqdsnc.cn/gtpzpzngkw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gtthpfyuzd.html

[Q70] 更新统计信息
来源：http://hz.wangdashe.top/gtsjsghubg.html

ANALYZE TABLE users;
来源：http://hz.andypj.xyz/gtahmwkhwi.html

[Q71] 查看建表语句
来源：http://hz.fengsongda.top/gtnvnhcbsn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuetiantiany.cn/gtqeyowyrr.html

[Q72] 查看索引
来源：http://hz.andypj.xyz/gtwpnkreqj.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtrzkjgsne.html

[Q73] 查看表状态
来源：http://hz.c1oappe.top/gtwlvhcolw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.svipenyu.cn/gtbmfpcjde.html

[Q74] 强制使用索引
来源：http://hz.sweek.top/gtotzyejji.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gzhubu.top/gtmatkzjzp.html

[Q75] 日期格式化
来源：http://hz.hfpthk.cn/gtdmtjerwv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gaohongyu789.top/gtairwkhrv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtuhfxfgug.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gtxwkpszho.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhengqikj.top/gtpasjsqak.html

[Q77] 时间加减
来源：http://hz.xylfe.cn/gtqlhtkveu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtnzitqutm.html

[Q78] 当前时间
来源：http://hz.xuanzx.com/gtbeptimhk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.havefunace.top/gtaltcnhph.html

[Q79] 字符串拼接
来源：http://hz.birdmap.top/gtdagxqmlj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.xuetiantiany.cn/gtuxdqaiha.html

[Q80] 字符串截取
来源：http://hz.sxryk.cn/gtiqecgcic.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yonumen.top/gtscsqwehl.html

[Q81] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtgsmgzjxz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhoulong.xyz/gtkvpnhlls.html

[Q82] 字符长度与字节长度
来源：http://hz.cheryme.top/gtebayboxy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sxryk.cn/gtcxoffimi.html

[Q83] 大小写转换
来源：http://hz.wangshuangyany.cn/gtdvsfevmb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtknvzzckm.html

[Q84] 去除首尾空格
来源：http://hz.cashguo.top/gtnmboxuaz.html

SELECT TRIM(name) FROM users;
来源：http://hz.ydzc1.top/gtynvcsecf.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtowznoolh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yueranfly.top/gtfrirevmo.html

[Q86] 读取 JSON 字段
来源：http://hz.guowangkeji.top/gtjrrbyrks.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gtffjumhkm.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gthlffxevj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhoulong.xyz/gtvinxzzsp.html

[Q88] 行转列（条件聚合）
来源：http://hz.sysykeji.top/gtturwcfte.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenzaomai.com/gtixjybvte.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tian-w.cn/gtzjaqpxfi.html

[Q89] 判断表是否存在
来源：http://hz.zhaomingkeji.xyz/gtiarpwqji.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cdnleiting.top/gtrsmugadj.html

[Q90] 生成序号列
来源：http://hz.pycfn.com/gtdcwwtddp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhongyouzk.top/gtukwgrmpm.html

================================================================================
来源：http://hz.iojbl.cn/gtavpemcjp.html

R. Bash 专题
来源：http://hz.jiagoushi.top/gtkmkuzqib.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtyoxdxlah.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtwdbcezzz.html

#!/usr/bin/env bash
来源：http://hz.chenzaomai.com/gtpdpbptdl.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gthadacwgi.html

[R02] 变量赋值与使用
来源：http://hz.jianghu66.top/gtggtwzryv.html

name="Tom"; echo "$name"
来源：http://hz.xinyue.icu/gtxkcftjai.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gthzqvhnwx.html

readonly PI=3.14
来源：http://hz.gotoacloud.top/gtcjfkhlbh.html

[R04] 位置参数
来源：http://hz.chenjidiqi.icu/gtcgcrgvix.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.iojbl.cn/gtbxayoygl.html

[R05] 参数默认值
来源：http://hz.hnxiangtu.top/gtfgvvzldg.html

name="${1:-default}"
来源：http://hz.hammf.cn/gtlvthngxk.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gthizvaehf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtdtmodyqs.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtmmuzeuha.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gtjkycgowh.html

[R08] 数值比较
来源：http://hz.guowangkeji.top/gtgqglehpf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.0kj1m.cn/gtjehnslxk.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtqiujobux.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtidkcprni.html

[R10] 正则匹配
来源：http://hz.ehwqpu.com/gtjtmqihmk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cqqwz.cn/gtdiueyywx.html

[R11] case 多分支
来源：http://hz.ybcxt.top/gtxzvlhfke.html

case "$1" in
来源：http://hz.0kj1m.cn/gtqjvahcnj.html

start) echo "启动" ;;
来源：http://hz.tian-w.cn/gtqpyyvoud.html

stop)  echo "停止" ;;
来源：http://hz.yangfankeji.com/gtgbtzzwtm.html

*)     echo "未知命令" ;;
来源：http://hz.zhijiandao.cn/gttmgllzsv.html

esac
来源：http://hz.wangshuangyany.cn/gtjdukyqyw.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtwjbfkfdj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jlsjyb.cn/gtshehlwwq.html

[R13] for 计数循环
来源：http://hz.yanxiufei.cn/gtdsiwxcpc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.daxiang520.top/gtrebcuklf.html

[R14] C 风格 for
来源：http://hz.pycfn.com/gtqptpsalr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtqeqjawyr.html

[R15] while 逐行读文件
来源：http://hz.jlsjyb.cn/gtydtkcjtf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtndaxsrdd.html

[R16] until 等待条件
来源：http://hz.yj20258888.top/gtoicxphpk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtitrynavz.html

[R17] 数组定义与取值
来源：http://hz.hfpthk.cn/gtglpaojuy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cucudq.cn/gtcxnbzobk.html

[R18] 遍历数组
来源：http://hz.yvedp.cn/gtjfittsco.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zycfv.cn/gtmvnmjozj.html

[R19] 数组长度
来源：http://hz.xuanzx.com/gtwgnsbbge.html

echo "${#arr[@]}"
来源：http://hz.ppjwa.cn/gtumjuchty.html

[R20] 关联数组（字典）
来源：http://hz.sufxvd.cn/gtlmzmbedu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.bjfxy.top/gtwiutuebc.html

[R21] 字符串长度
来源：http://hz.yj20258888.top/gtmkjxichu.html

echo "${#s}"
来源：http://hz.jqgfzy.top/gtwjqxiqut.html

[R22] 截取子串
来源：http://hz.zhongyouzk.top/gtdlmsrcrn.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtkjmzzjrk.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtfiidpqmg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tanke756.top/gtbhnezvlg.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtcgpmcfgq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dashuyun.cn/gtfpnqtdxt.html

[R25] 去后缀 / 去前缀
来源：http://hz.sxryk.cn/gtyybaxyow.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtrqjjlisz.html

[R26] 命令替换
来源：http://hz.birdmap.top/gttwjmwdru.html

now=$(date +%F); echo "$now"
来源：http://hz.nwbrower.top/gtlqmknsxi.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gtuloajlsc.html

echo $((1 + 2 * 3))
来源：http://hz.fzhhl.top/gtjkzgfvau.html

[R28] 浮点运算
来源：http://hz.ppjwa.cn/gtfiohhehp.html

echo "scale=2; 10/3" | bc
来源：http://hz.yonumen.top/gtnuycqjva.html

[R29] 定义函数
来源：http://hz.yueranfly.top/gtxpmotanq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yongpay.top/gtjtpjswgj.html

[R30] 函数返回状态码
来源：http://hz.tian-w.cn/gtrdambgbl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jianghu66.top/gthhwebmay.html

[R31] 局部变量
来源：http://hz.jinqigufen.top/gtkdmmzsxb.html

f() { local x=1; echo "$x"; }
来源：http://hz.shanyushiyangkeji.top/gtxwjjiqqq.html

[R32] 参数个数校验
来源：http://hz.c1oappe.top/gtigozevca.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangdashe.top/gtnlwnpetf.html

[R33] 捕获错误并提示行号
来源：http://hz.sufxvd.cn/gtannkkxur.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtyeupunoe.html

[R34] 退出时清理
来源：http://hz.yj20258888.top/gtofrnajcc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinyuanbaomall.cn/gtmcnotudf.html

[R35] 后台执行并等待
来源：http://hz.jinghuilouyu.cn/gtnmbuxuif.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sweek.top/gtzchllfij.html

[R36] 并发执行多个任务
来源：http://hz.jqgufenzy.top/gtizhugbfo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtzxbhnlhc.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtotsyqebo.html

files=$(ls -1)
来源：http://hz.yj202588.top/gtstlyxvrj.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtubsizxqm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtbiillggz.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gtwlanhrer.html

cmd > out.log 2>&1
来源：http://hz.zdqjudy.top/gtazmgriqt.html

[R40] 追加写日志
来源：http://hz.hysaishi.cn/gtjrsmmngb.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gtzvqezfhy.html

[R41] 丢弃输出
来源：http://hz.zdqjudy.top/gtdpykzfcf.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtoxmdmcmy.html

[R42] 输入重定向
来源：http://hz.daria6918.cn/gtywvzgmmi.html

wc -l < a.txt
来源：http://hz.jianghu66.top/gtuncyajrl.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtxdcvgmwh.html

find . -name "*.log" -type f
来源：http://hz.c1oappe.top/gtdkofncgz.html

[R44] 按修改时间查找
来源：http://hz.nanxinkj.top/gtvqjakolx.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtftmujgjv.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gtpzexaydb.html

find . -name "*.tmp" -delete
来源：http://hz.zhaomingkeji.xyz/gtojgwqcye.html

[R46] 递归替换文件内容
来源：http://hz.hysaishi.cn/gtwiljmtls.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.feifeiyinyue.top/gtgrzaihca.html

[R47] sed 单行替换
来源：http://hz.bjfxy.top/gthjyeemjf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhoulong.xyz/gtmtaxfawx.html

[R48] awk 取指定列
来源：http://hz.haohaochexian.top/gtypwcbwsu.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhixingplan.top/gtobojgffx.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtsjcjxkpy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cucudq.cn/gtsnvjrand.html

[R50] awk 求和
来源：http://hz.xinyue.icu/gtedywzxpf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gtxabieqiu.html

[R51] 排序去重取前几
来源：http://hz.fengsongda.top/gtsdghhobk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtngyhfxar.html

[R52] 统计行数
来源：http://hz.jinqigfzy.top/gtpbnbvrms.html

wc -l a.txt
来源：http://hz.quarkkingdee.top/gtmywekjqc.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtvgljkdws.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuanzhike.top/gthgmmcerd.html

[R54] 比较两个文件
来源：http://hz.xylfe.cn/gtfvmcudjm.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gtnhlijdjv.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtwzjjhhbr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pycfn.com/gtflpwigng.html

[R56] 远程拷贝
来源：http://hz.cheryme.top/gtlaobhteu.html

scp file user@host:/path/
来源：http://hz.ydjk.org.cn/gtnraaycqw.html

[R57] 远程执行命令
来源：http://hz.jyoumei.cn/gtepgtxupe.html

ssh user@host 'uptime'
来源：http://hz.xuetiantiany.cn/gtruuxgscc.html

[R58] 下载文件
来源：http://hz.aizwys.cn/gtvngbgcdc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cashguo.top/gtiykkjcze.html

[R59] 发 POST JSON
来源：http://hz.cdnleiting.top/gtwrukdczj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gtpuhwqbfm.html

[R60] 只看 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtcrjpbpif.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.316326.xyz/gtrxkqicbw.html

[R61] 磁盘占用
来源：http://hz.tianlin.xyz/gtpwlnecom.html

df -h;  du -sh *
来源：http://hz.xziqi.cn/gtizvdaoqy.html

[R62] 找最占空间的文件
来源：http://hz.zhaomingkeji.xyz/gtkzazkwip.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangtech.top/gtvkyjlyie.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtrnpmdrwh.html

free -h;  ps aux | grep nginx
来源：http://hz.zhengqikj.top/gtrueiqofv.html

[R64] 结束进程
来源：http://hz.hammf.cn/gtisnpyqys.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtweardxjt.html

[R65] 查看端口占用
来源：http://hz.guannengcc.top/gtcnnbrqad.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.meibo888.top/gtkmnahhpp.html

[R66] 定时任务
来源：http://hz.havefunace.top/gtzgpsjwxu.html

crontab -e;  crontab -l
来源：http://hz.c1oappe.top/gtsbgqpncb.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtngqrjdvk.html

openssl rand -hex 16
来源：http://hz.shanyushiyangkeji.top/gttnlqnimb.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtfsahkwzd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtbunliygu.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtarvsmtap.html

head -c 16 /dev/urandom | base64
来源：http://hz.wangdashe.top/gtuepncupd.html

[R70] 时间戳与互转
来源：http://hz.ehwqpu.com/gtzonycrik.html

date +%s;  date -d @1700000000
来源：http://hz.9152youxi.cn/gtjtnwhelm.html

[R71] 日期格式化
来源：http://hz.tianlin.xyz/gtgxwwazil.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aizwys.cn/gtvxvyumyh.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gtrqaoolmn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtzjylwqxr.html

[R73] 分割大日志
来源：http://hz.yj20258.top/gtassuahao.html

split -l 1000 big.log part_
来源：http://hz.cqqwz.cn/gtkdktxaax.html

[R74] 批量重命名
来源：http://hz.chenjidiqi.icu/gtwtizalyh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jlsjyb.cn/gtwfkefkqy.html

[R75] 导出环境变量
来源：http://hz.hywenlv.cn/gtfvrfufzy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gogol.net.cn/gtljseqkxz.html

[R76] 使用临时文件
来源：http://hz.zhixingplan.top/gtzoorbmyo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtktbdtezd.html

[R77] 读取用户输入
来源：http://hz.zhaomingkeji.xyz/gtusakxowa.html

read -rp "请输入: " ans
来源：http://hz.zhixingplan.top/gtlgedzgnt.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtyeylaczn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gtnepqnkkq.html

[R79] 解析命令行选项
来源：http://hz.sysykeji.top/gtruypmrrq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gogol.net.cn/gtjgfsxzuk.html

[R80] 查看脚本执行耗时
来源：http://hz.ehwqpu.com/gtetycjtbw.html

time ./run.sh
来源：http://hz.redwolf501.top/gtqratufyw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqqmielnv.html

S. C / C++ 专题
来源：http://hz.sxryk.cn/gtumtmqxta.html

================================================================================
来源：http://hz.ydzc1.top/gtofbtnvfo.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtjnmgaleo.html

#include <stdio.h>
来源：http://hz.yongpay.top/gtnbghvgoo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.c1oappe.top/gtakcpxmbd.html

[S02] C：变量与格式化输出
来源：http://hz.daxiang520.top/gtocodhnvc.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtnjqyblxm.html

[S03] C：读入整数
来源：http://hz.dashuyun.cn/gtswwrpsxm.html

int x; scanf("%d", &x);
来源：http://hz.yj20258.top/gtuofcteli.html

[S04] C：字符串复制
来源：http://hz.jinqigfzy.top/gtyremttva.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigufen.top/gtxqychnrd.html

[S05] C：字符串长度
来源：http://hz.kuanghao11.cn/gtwrndjllo.html

strlen(s)
来源：http://hz.yanxiufei.cn/gtdrfkkwtd.html

[S06] C：字符串比较
来源：http://hz.ybcxt.top/gtfparlguo.html

strcmp(a, b) == 0
来源：http://hz.jiagoushi.top/gtuvysffnb.html

[S07] C：数组遍历求和
来源：http://hz.feifeiyinyue.top/gtszgavief.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhoulong.xyz/gtpsvwmzvd.html

[S08] C：动态内存分配与释放
来源：http://hz.jianghu66.top/gtjtkgffbr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gzhubu.top/gtcwyolatj.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtcjnpadwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.52xcode.cn/gtlushaswb.html

[S10] C：指针与解引用
来源：http://hz.ybcxt.top/gtwxveepqz.html

int *p = &a;  *p = 5;
来源：http://hz.zycfv.cn/gtwluczodw.html

[S11] C：逐行读文件
来源：http://hz.zhiwuduotai.top/gtssqchspl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xingfuxueyuan.xyz/gtofhxjwvu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.quarkkingdee.top/gtedgycysi.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtmuoxjsre.html

[S12] C：写文件
来源：http://hz.ppjwa.cn/gtvjdogiwe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuxming.cn/gtvpmrwjrh.html

[S13] C：宏定义
来源：http://hz.daria6918.cn/gtidllyfel.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.havefunace.top/gtmexxhzvk.html

[S14] C：枚举
来源：http://hz.ivvv.top/gttfltpsel.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigufen.top/gtscziywob.html

[S15] C：类型转换
来源：http://hz.yvedp.cn/gtvjzptivv.html

(double) a / b
来源：http://hz.chenzaomai.com/gtetmfgeoi.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtpwmvnvcv.html

x |= (1 << 3);
来源：http://hz.zdqjudy.top/gtmmoxrtad.html

[S17] C：安全拼接字符串
来源：http://hz.yj202588.top/gtwpmvmavo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgufenzy.top/gtpvnoeoof.html

[S18] C：命令行参数
来源：http://hz.jqgfzy.top/gtzevrkfjq.html

int main(int argc, char **argv)
来源：http://hz.chenzaomai.com/gtlwzxjywx.html

[S19] C：快速排序
来源：http://hz.cashguo.top/gtwxjmmghy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtfqpknlyg.html

[S20] C：二分查找
来源：http://hz.bjfxy.top/gtxjisefhc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtqlecniaf.html

[S21] C：字符类别判断
来源：http://hz.cashguo.top/gtokjulkpu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daria6918.cn/gtnvnrozmy.html

[S22] C：字符串转数字
来源：http://hz.jinghuilouyu.cn/gtzbbcsbey.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hnxiangtu.top/gtbvfrqfze.html

[S23] C：随机数
来源：http://hz.zdqjudy.top/gtdtpwicct.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtcvqjafpg.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtqugsyyfl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yongpay.top/gtbmdwpsvf.html

[S25] C：内存拷贝
来源：http://hz.hfpthk.cn/gtwggnsxbd.html

memcpy(dst, src, n);
来源：http://hz.shuidangran.top/gtsykusjol.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gtfdbbonho.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gtzcwoftss.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtnyperzqk.html

const double PI = 3.14159;
来源：http://hz.yuxming.cn/gteutwrvae.html

[S28] C：静态变量
来源：http://hz.sufxvd.cn/gtelchbfuq.html

static int counter = 0;
来源：http://hz.yuxming.cn/gtfdaqigoa.html

[S29] C：变参函数
来源：http://hz.bjfxy.top/gtwzcopcci.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.redwolf501.top/gtoiiifsfi.html

[S30] C：头文件保护
来源：http://hz.jyoumei.cn/gtlcpbljui.html

#ifndef X_H
来源：http://hz.zhaomingkeji.xyz/gteejsafka.html

#define X_H
来源：http://hz.birdmap.top/gtztfrrzyh.html

#endif
来源：http://hz.tian-w.cn/gtffyivbbs.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtfpihuwfo.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtufrgpxxd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ivvv.top/gtivberglx.html

[S32] C++：字符串
来源：http://hz.sweek.top/gtfosimjdr.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtmjsjhsqp.html


<!-- 参考信息 -->